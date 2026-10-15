---
description: >-
  Run TV Rename's scans, actions and updates from a shortcut, a batch file or
  Windows Task Scheduler, without clicking through the window.
---

# Command Line

Everything on this page can also be done from TV Rename's own window. The command line is for when you want it to happen without you: a desktop shortcut that starts a scan, a batch file, or a task that runs overnight.

## Before you start

TV Rename installs to `C:\Program Files (x86)\TVRename` unless you chose a different folder when installing it. Because that path contains spaces, it must be in quotes. Switches go after it, separated by spaces, and are not case sensitive.

| Where            | How                                                                                                                      |
| ---------------- | ------------------------------------------------------------------------------------------------------------------------ |
| Command Prompt   | `"C:\Program Files (x86)\TVRename\TVRename.exe" /recentscan`                                                             |
| PowerShell       | Put `&` in front: `& "C:\Program Files (x86)\TVRename\TVRename.exe" /recentscan`                                         |
| Desktop shortcut | Right-click the shortcut, choose **Properties**, and add the switches to the end of **Target**, after the closing quote. |
| Task Scheduler   | **Program/script**: the quoted path above. **Add arguments**: the switches.                                              |

The examples below shorten the path to `TVRename.exe`.

## Common tasks

| You want to                                                                        | Command                                                                   |
| ---------------------------------------------------------------------------------- | ------------------------------------------------------------------------- |
| Open TV Rename and run a recent scan, then look at the results yourself            | `TVRename.exe /recentscan`                                                |
| Scan everything, carry out all the actions, then close                             | `TVRename.exe /scan /doall /quit`                                         |
| Run overnight from Task Scheduler with nothing on screen: update, scan, act, close | `TVRename.exe /hide /quickupdate /recentscan /ignoremissing /doall /quit` |
| Tell TV Rename, already open, to scan now                                          | `TVRename.exe /recentscan`                                                |
| Tell TV Rename, already open, to save its settings                                 | `TVRename.exe /save`                                                      |

{% hint style="warning" %}
`/doall` carries out **every** action in the list, including any you have unticked in the Scan tab. Run a scan without it first, and look at the results, until you are happy with what TV Rename does with your library.
{% endhint %}

## How TV Rename handles the switches

**Order.** Whatever order you type the switches in, TV Rename always works through them in this order:

1. `/hide`
2. `/quickupdate`, `/forceupdate`, `/forcerefresh`
3. `/scan`, `/quickscan`, `/recentscan`
4. `/doall`
5. `/save`
6. `/export`
7. `/quit`

So `/quit /scan` still scans first and quits afterwards.

**If TV Rename is already open.** Only one copy of TV Rename runs at a time. Running it again passes the switches to the open window, which does the work, and the second copy closes straight away. `/createmissing`, `/ignoremissing` and `/norenamecheck` then apply to that one request only.

This also means `/doall` sent to an open window carries out whatever is already in its Scan tab, even without a scan switch.

## Switch reference

### Scanning and actions

| Switch          | What it does                                                                                                                                                                       |
| --------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **/scan**       | Run a full scan. A scan only builds the list of actions; nothing on disk changes unless `/doall` is also given. See [Scanning](../guides/features/scanning.md) for the scan types. |
| **/recentscan** | Run a recent scan: shows with an episode aired in the last few days.                                                                                                               |
| **/quickscan**  | Run a quick scan.                                                                                                                                                                  |
| **/doall**      | Carry out all the actions in the list. Use it with a scan switch, otherwise a freshly started TV Rename has nothing to do.                                                         |
| **/export**     | Run the exports you have set up in [Preferences](../menu/preferences.md#episode-export).                                                                                           |
| **/quit**       | Close TV Rename once everything else has finished. Works on a hidden copy and on an open window.                                                                                   |

### Updating show and movie information

| Switch            | What it does                                                                                      |
| ----------------- | ------------------------------------------------------------------------------------------------- |
| **/quickupdate**  | Download recent changes from TheTVDB, TMDB and TV Maze.                                           |
| **/forceupdate**  | Check that the TheTVDB and TMDB information is up to date.                                        |
| **/forcerefresh** | Download everything again for every show and movie. This can take a long time on a large library. |
| **/save**         | Save TV Rename's settings and downloaded information now.                                         |

### Running without anyone watching

| Switch          | What it does                                                                                                                                                                                                                                                                                                            |
| --------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **/hide**       | Run with no window, splash screen, notification area icon or pop-ups. Missing folders are skipped unless `/createmissing` is also given. TV Rename does **not** close by itself: include `/quit`, or it keeps running in the background until you end it in Task Manager. Sent to an open window, `/hide` minimises it. |
| **/unattended** | Show the window but no pop-ups that wait for you to click; errors and warnings go to the [log](logs-and-configuration.md#log-files) instead. The "missing folder" question can still appear, so add `/ignoremissing` or `/createmissing` when nobody will be there to answer it.                                        |

### Missing folders and renaming

| Switch             | What it does                                              |
| ------------------ | --------------------------------------------------------- |
| **/createmissing** | Create any missing season folders without asking.         |
| **/ignoremissing** | Skip missing folders this time without asking.            |
| **/norenamecheck** | When sent to an open window, scan without renaming files. |

### Other

| Switch                 | What it does                                                                                                                                                                                        |
| ---------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **/recover**           | Open a window to restore an earlier copy of your settings or downloaded show information. Normally this only appears by itself when the current files are damaged.                                  |
| **/userfilepath:PATH** | Keep the settings files in a different folder, for example `/userfilepath:D:\TVRenameSettings`. See [Logs & Configuration](logs-and-configuration.md#configuration-files) for what those files are. |
| **/?**                 | Write the list of switches to the log, then exit without starting TV Rename.                                                                                                                        |
