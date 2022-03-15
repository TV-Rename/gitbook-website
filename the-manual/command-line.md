---
description: >-
  A number of TV Rename’s functions can be accessed using the command line. If
  TV Rename is already running any CLI activity will be directed towards the
  running instance.
---

# Command Line

### Main Options

**/scan**

Tell TV Rename to run a full scan.

**/recentscan**

Tell TV Rename to run a recent scan.

**/quickscan**

Tell TV Rename to run a quick scan.

**/doall**

Tell TV Rename execute all the actions it can (User needs to specify which scan type is required otherwise there will be no actions to complete - choose from above scan options on the command line).

**/export**&#x20;

Tell TV Rename do any configured exports.

**/quit**

Tell a hidden TV Rename session to exit.

### Updates & Saving <a href="#hidden-behaviour" id="hidden-behaviour"></a>

**/forcerefresh**&#x20;

will refresh all TVDB, TMDB and TV Maze information

**/forceupdate**&#x20;

will verify TVDB & TMDB information is up to date

**/quickupdate**

will do a quick update from TVDB, TMDB and TV Maze

**/save**

Tell a running TV Rename session to save its caches.

### Hidden Behaviour <a href="#hidden-behaviour" id="hidden-behaviour"></a>

**/hide**

Hides the User Interface and associated message boxes from view.\
Defaults to not add missing folders (providing “/createmissing” is not set).\
Exits once actions complete.

**/unattended**

This option means that the main UI is shown, but does not put up any blocking UI elements that need hunman interaction. Mainly this means that error and warning are just recorded in the log and the user does not get a message box notification.

### Override Options <a href="#override-options" id="override-options"></a>

**/createmissing**

Creates folders if they are missing.

**/ignoremissing**

Ignore missing folders.

**/norenamecheck**

Allows a request to an existing TV Rename session to scan without renaming.

### Settings Files <a href="#settings-files" id="settings-files"></a>

**/recover**

Recover will load a dialog box that enables the user to recover a prior TVDB.xml or TVRenameSettings.xml file. (Normally this dialog would only appear if the current settings are corrupted.)

**/userfilepath:BLAH**

Sets a custom folder path for the settings files

**/?**

Displays help information in the logs
