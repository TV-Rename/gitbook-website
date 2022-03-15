# Scan

TV Rename can scan your media library looking for missing or outdated files and will try to repair any issues it finds automatically.

There are three types of scan available : -

| **Full**   | A full scan of all shows and seasons.                                                                                                                                                       |
| ---------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Recent** | A Scan of all the shows that have aired recently.                                                                                                                                           |
| **Quick**  | Scan the shows that have aired recently and have a missing episode in the library. Also check the locations specified in _Options>Preferences>Search Folders_ for any matching media files. |

As with other tabs, “recent” is taken as being the number of days counted as recent indicated in the **Options>Preferences** [_**General**_](https://www.tvrename.com/manual/options#the-general-tab) tab.

_**Scan**_ indicates where there are gaps in your library. The result of a typical scan is shown below.

![The Scan Tab](https://www.tvrename.com/assets/images/main-window/scan-03.png)

The scan indicates that there a number of missing episodes, a file in the media library that needs to be renamed, a file that has been downloaded and is waiting to be moved to the media library and be renamed in the process and a duplicate file that can be removed.

Looking at the missing episodes first; even here TV Rename is “trying to help”. Note that each entry has a magnifying glass icon to the left of the row. Single clicking one of these rows and then clicking the `Web Search` button (in this case “Zooqle”) will launch a search for the indicated file (configured in [**Options>Search Engines**](https://www.tvrename.com/manual/options#search-engines)). Double clicking one of these rows will launch the same web search. You an also select multiple rows and then click the `Web Search` button to launch a browser with multiple tabs, one for each highlighted row.

If you’re having trouble finding what you’re searching for you can change the search engine to another in the [**Options>Search Engines**](https://www.tvrename.com/manual/options#search-engines) list by clicking the `▼` button next to “Web Search” and selecting a different entry.

In addition to the files to be searched for, the _**Scan**_ tab is also showing that there is one file to be renamed and one file to be copied or moved (see the **Options>Preferences** [_**Scan Options**_](https://www.tvrename.com/manual/user/options#scan-options) tab). Note both items have a tick in the box icon to the left of each row.

![The Choose File prompt](https://www.tvrename.com/assets/images/main-window/scan-choose-file-01.png)If the “Update episodes when higher quality ones found” box is ticked in **Options>Preferences** [_**Scan Options**_](https://www.tvrename.com/manual/user/options#scan-options) and there are two versions of an episode file in the library and/or download location you will be prompted to choose which file to keep when the scan completes as illustrated…

When the `Do Checked` button is clicked everything ticked will be processed.

Note that there are some tick boxes to the right of the buttons. These give you course control over the ticked items, it this case we can toggle everything to be moved and/or everything to be renamed on and off.

There are also a number of useful options available in the right-click menu here.

Selecting files in the main scan panel and clicking `Ignore Selected` will remove them from the system (permanently unless they are removed from the ignore list - see [**Options>Ignore  List**](https://www.tvrename.com/manual/user/options#ignore-list)).

Selecting files in the main scan panel and clicking `Revert to Missing` will mark (and list) them as missing. (If they are within the date range of “Aired in the last…” in the _**When to watch**_ tab they will also be shown as missing there.

Selecting files in the main scan panel and clicking `Remove Selected` will temporarily remove them from the scan tab. They will re-appear when the scan is re-run.

In addition you can toggle individual items on or off by clicking directly on their tick boxes.

Once you are happy with everything selected click on `Do Checked` and the Copy/Move/Rename process will start.

![The Progress Pane](https://www.tvrename.com/assets/images/main-window/progress-01.png)While files are being copied and/or moved, this dialog is shown. Click `Pause` to temporarily pause the copy/move operation. Click it again to resume. Clicking `Cancel` will stop the operation immediately. The disk space shown is for the drive that the current file is being copied/moved to.
