# Technical Guide

### Configuration Files <a href="#configuration-files" id="configuration-files"></a>

By default, all the configuration information and locally cached data from [TheTVDB](http://thetvdb.com) is stored in a series of XML files under the users Application folder (unless overridden using the command line option /userfilepath). They are stored at: -

> \Users\\\<user-name>\AppData\Roaming\TVRename\TVRename\2.1

**If you wish to make a backup of your TV Rename setup a copy of this folder is all you need!**

It contains:

| **TVRenameSettings.xml** | Everything else not mentioned is stored in here. All your shows, media library paths, folder structures and settings. This is only overwritten when you choose **File>Save**. |
| ------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **TheTVDB.xml**          | The locally cached tvdb.com show season and episode information for everything listed in the _**My Shows**_ tab.                                                              |
| **Layout.xml**           | TV Rename’s window position and size as well as column widths.                                                                                                                |
| **Statistics.xml**       | TV Rename’s historical statistics.                                                                                                                                            |
| **Languages.xml**        | TV Rename’s cache of possible languages to cover.                                                                                                                             |

And stores the following backups (10 of each):

| **TVRenameSettings.xml.0-9** | Backup copies of TV Rename settings.xml (FIFO).                                                                                                                        |
| ---------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **TheTVDB.xml.0-9**          | A maximum of ten backup copies of TheTVDB.xml file. A new file gets created here every time the system gets updates from theTVDB on a first-in-first-out (FIFO) basis. |

### Log Files <a href="#log-files" id="log-files"></a>

The main active log file is available from the **Help>Log** menu option. Note that the application only logs to the screen once it’s opened. If you want to see the full log then click on ‘View Full Log’ and the whole thing is opened up. The log window can be moved and the rest of the application used as normal.

The current log file (TVRename.log) can be found in: -

> \Users\\\<username>\AppData\Roaming\TV Rename\log\\

Log files are rotated into an “archive” folder (in the same location as TVRename.log) every time TV Rename is run or every 24 hours, whichever is sooner.

As with **tvdb.xml** and **settings.xml** a maximum of ten backup copies of the log file are kept (**TVRename00.log** - **TVRename09.log**) on a first-in-first-out (FIFO) basis.

Logging uses NLog. The configuration file ([NLog.config](https://github.com/TV-Rename/tvrename/blob/master/TVRename%23/NLog.config)) is stored in the TV Rename program folder.

You can read the [NLog Wiki](https://github.com/nlog/NLog/wiki/Configuration-file) for guidance on how to adjust the configuration file to collect more information.

When raising a bug please include a log file that illustrates the issue if you can, it will help us find a solution quickly.

### The Registry <a href="#the-registry" id="the-registry"></a>

The only information TV Rename stores in the registry is installation information which is used by Windows “Apps and Features” to un-install the program. But hey, why would you want to do that?

It also sets the compatability status of IE in the registry by settign a key at Software\Microsoft\Internet Explorer\Main\FeatureControl\FEATURE\_BROWSER\_EMULATION so that the latest version of IE is used to render the graphical side of the application.

### Source Code <a href="#source-code" id="source-code"></a>

You can find TV Rename’s source code (along with executables and this website) in [The TV Rename GitHub Repository](https://github.com/TV-Rename/tvrename).

### Development Links <a href="#development-links" id="development-links"></a>

* You can find the Developers Wiki [here](https://github.com/TV-Rename/tvrename/wiki)…
* For the longer term you can visit the “[Roadmap](https://github.com/TV-Rename/tvrename/milestones?direction=asc\&sort=due\_date\&state=open)” which lists the proposed Milestones (a high level view of whats planned for when).
* In addition there is a [Developers Forum in Google Groups](https://groups.google.com/forum/#!forum/tv-rename-development) which you can request access to.
* The legacy forum can be [accessed](http://old.tvrename.com/bbold/) in read-only mode for background and history about the project

### Framework <a href="#framework" id="framework"></a>

TV Rename uses the Microsoft .NET Framework. The installer will check for its presence and let you know if any action is needed. It’s a free download from [Microsoft](https://www.microsoft.com/net/download/windows).

### Credits <a href="#credits" id="credits"></a>

TV Rename pulls data from [TheTVDB.com](http://thetvdb.com) using their API. **Please visit their site, register, and help out by contributing information and artwork for TV Series and Episodes.**

It also uses: -

* [Json.NET](https://www.newtonsoft.com/json),
* [AlphaFS](http://alphafs.alphaleonis.com) for advanced .NET file operations,
* [NLog](http://nlog-project.org) open-source logging for .NET,
* [SourceGrid](https://sourcegrid.codeplex.com),
* TVRename has seen significant speed improvements as a result of using: -
  * Red Gate’s [ANTS Performance Profiler](https://www.red-gate.com/products/dotnet-development/ants-performance-profiler/)
  * JetBrains’ [dotTrace](https://www.jetbrains.com/profiler)
  * JetBrains’ [ReSharper](https://www.jetbrains.com/resharper)

And thanks to:\
Vecteezy! Vector Art for our cool [Retro Television Logo](https://www.vecteezy.com/vector-art/73089-retro-television) - Vectors by [www.vecteezy.com](https://www.vecteezy.com).
