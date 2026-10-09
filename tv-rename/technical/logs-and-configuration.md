# Logs & Configuration

### Configuration Files <a href="#configuration-files" id="configuration-files"></a>

By default, all the configuration information and locally cached data from [TheTVDB](http://thetvdb.com/) is stored in a series of XML files under the users Application folder (unless overridden using the command line option /userfilepath). They are stored at: -

> \Users\\\<user-name>\AppData\Roaming\TVRename\TVRename\2.1

**If you wish to make a backup of your TV Rename setup a copy of this folder is all you need!**

It contains:

| **TVRenameSettings.xml**                                                                        | Everything else not mentioned is stored in here. All your shows, media library paths, folder structures and settings. This is only overwritten when you choose **File>Save**. |
| ----------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <p><strong>TheTVDB.xml</strong><br><strong>TMDB.xml</strong><br><strong>TVMaze.xml</strong></p> | The locally cached data about movies, shows seasons and episodes for everything listed in the _**TV Shows**_ tand **Movies** tabs.                                            |
| **Layout.xml**                                                                                  | TV Rename’s window position and size as well as column widths.                                                                                                                |
| **Statistics.xml**                                                                              | TV Rename’s historical statistics.                                                                                                                                            |
| **Languages.xml**                                                                               | TV Rename’s cache of possible languages to cover.                                                                                                                             |
| **State.xml**                                                                                   |                                                                                                                                                                               |

And stores the following backups (10 of each):

| **TVRenameSettings.xml.0-9**                                                                                | Backup copies of TV Rename settings.xml (FIFO).                                                                                                                                                                       |
| ----------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <p><strong>TheTVDB.xml.0-9</strong><br><strong>TMDB.xml.0-9</strong><br><strong>TVMaze.xml.0-9</strong></p> | A maximum of ten backup copies of the XML cache files. A new file gets created here every time the system gets updates from [data sources](../help-and-support/data-sources.md) on a first-in-first-out (FIFO) basis. |

### Log Files <a href="#log-files" id="log-files"></a>

The main active log file is available from the **Help>Log** menu option. Note that the application only logs to the screen once it’s opened. If you want to see the full log then click on ‘View Full Log’ and the whole thing is opened up. The log window can be moved and the rest of the application used as normal.

The current log file (TVRename.log) can be found in: -

> \Users\\\<username>\AppData\Roaming\TV Rename\log\\

Log files are rotated into an “archive” folder (in the same location as TVRename.log) every time TV Rename is run or every 24 hours, whichever is sooner.

As with **tvdb.xml** and **settings.xml** a maximum of twenty backup copies of the log file are kept in files with a number suffix (eg **TVRename\<nn>.log**) on a first-in-first-out (FIFO) basis.

Logging uses NLog. The configuration file ([NLog.config](https://github.com/TV-Rename/tvrename/blob/master/TVRename%23/NLog.config)) is stored in the TV Rename program folder.

You can read the [NLog Wiki](https://github.com/nlog/NLog/wiki/Configuration-file) for guidance on how to adjust the configuration file to collect more information.

When raising a bug please include a log file that illustrates the issue if you can, it will help us find a solution quickly.

### Cache and Supporting Logs <a href="#the-registry" id="the-registry"></a>

| **log/cef-debug.log** | Specific log file related to the in-built broswer                                                                 |
| --------------------- | ----------------------------------------------------------------------------------------------------------------- |
| **audit/\*.json**     | If enabled, audit logs the downloaded information from the upstream data sources. Can be safely deleted if needed |
| **cache/\***          | Cache that the built-in browser uses to speed its operation. Can be safely deleted.                               |

### The Registry <a href="#the-registry" id="the-registry"></a>

The only information TV Rename stores in the registry is installation information which is used by Windows “Apps and Features” to un-install the program.
