---
description: >-
  A number of TV Rename’s functions can be accessed using the command line. If
  TV Rename is already running any CLI activity will be directed towards the
  running instance.
---

# Command Line

### Main Options

<table><thead><tr><th width="211"></th><th></th></tr></thead><tbody><tr><td><strong>/scan</strong></td><td>Tell TV Rename to run a full scan.</td></tr><tr><td><strong>/recentscan</strong></td><td>Tell TV Rename to run a recent scan.</td></tr><tr><td><strong>/quickscan</strong></td><td>Tell TV Rename to run a quick scan.</td></tr><tr><td><strong>/doall</strong></td><td>Tell TV Rename execute all the actions it can (User needs to specify which scan type is required otherwise there will be no actions to complete - choose from above scan options on the command line).</td></tr><tr><td><strong>/export</strong></td><td>Tell TV Rename do any configured exports.</td></tr><tr><td><strong>/quit</strong></td><td>Tell a hidden TV Rename session to exit.</td></tr></tbody></table>

### Updates & Saving <a href="#hidden-behaviour" id="hidden-behaviour"></a>

<table><thead><tr><th width="211"></th><th></th></tr></thead><tbody><tr><td><strong>/forcerefresh</strong></td><td>will refresh all TVDB, TMDB and TV Maze information</td></tr><tr><td><strong>/forceupdate</strong></td><td>will verify TVDB &#x26; TMDB information is up to date</td></tr><tr><td><strong>/quickupdate</strong></td><td>will do a quick update from TVDB, TMDB and TV Maze</td></tr><tr><td><strong>/save</strong></td><td>Tell a running TV Rename session to save its caches.</td></tr></tbody></table>

### Hidden Behaviour <a href="#hidden-behaviour" id="hidden-behaviour"></a>

<table><thead><tr><th width="201"></th><th></th></tr></thead><tbody><tr><td><strong>/hide</strong></td><td>Hides the User Interface and associated message boxes from view.<br>Defaults to not add missing folders (providing “/createmissing” is not set).<br>Exits once actions complete.</td></tr><tr><td><strong>/unattended</strong></td><td>This option means that the main UI is shown, but does not put up any blocking UI elements that need hunman interaction. Mainly this means that error and warning are just recorded in the log and the user does not get a message box notification.</td></tr></tbody></table>

### Override Options <a href="#override-options" id="override-options"></a>

<table><thead><tr><th width="200"></th><th></th></tr></thead><tbody><tr><td><strong>/createmissing</strong></td><td>Creates folders if they are missing.</td></tr><tr><td><strong>/ignoremissing</strong></td><td>Ignore missing folders.</td></tr><tr><td><strong>/norenamecheck</strong></td><td>Allows a request to an existing TV Rename session to scan without renaming.</td></tr></tbody></table>

### Other <a href="#settings-files" id="settings-files"></a>

<table><thead><tr><th width="200"></th><th></th></tr></thead><tbody><tr><td><strong>/recover</strong></td><td>Recover will load a dialog box that enables the user to recover a prior TVDB.xml or TVRenameSettings.xml file. (Normally this dialog would only appear if the current settings are corrupted.)</td></tr><tr><td><strong>/userfilepath:BLAH</strong></td><td>Sets a custom folder path for the settings files</td></tr><tr><td><strong>/?</strong></td><td>Displays help information in the logs</td></tr></tbody></table>

