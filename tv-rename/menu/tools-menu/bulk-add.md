# Bulk Add

## Bulk Add Shows <a href="#bulk-add-shows" id="bulk-add-shows"></a>

<figure><img src="https://3508557057-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2Fx0gPeIfHpbgTioNust1M%2Fuploads%2FcIhdVSQXNqCF1qVKoU9I%2Fimage.png?alt=media&#x26;token=6d67b7df-3ddb-449a-a339-abe82336432c" alt=""><figcaption></figcaption></figure>

This is where you tell TV Rename about the location(s) of your media library. Additionally you can check these locations for new folders unknown to TV Rename and quickly scan and add them to the _**TV Shows**_ tab.

Before using this tool, check that your preferred renaming style is set in [_Options>Filename Template Editor_](../options-menu/filename-template-editor.md).

`Add` (or Drag-and-Drop) folders to the _**Folders:**_ tab. Click the `Check >>` button, and TV Rename will recursively search through the new folders looking for new TV shows. Once this is complete, if anything new is found, the _**Scan Results**_ tab will appear populated with the paths to any newly found shows, it will also identify the folder structure of the show (“Flat” - everything in one folder or “Folder per season”).

<figure><img src="https://3508557057-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2Fx0gPeIfHpbgTioNust1M%2Fuploads%2FgEGZlKS8pZnmDE0Rjm8U%2Fimage.png?alt=media&#x26;token=9df9c295-6f28-4faf-ba08-812b08b2e9cf" alt=""><figcaption></figcaption></figure>

The system inspects each folder and if it contains any sub-folders that look like they are a season it assumes that they are structured in separate folders per season. TV Rename looks for any folders that start with any of the ‘season words’ entered in the preferences, with the default season word (again entered in preferences) and (if configured) any of the words used as season folder names for any of the shows in your library. The preferences for this function are specified [here](../preferences.md#the-files-and-folders-tab) and [here](../preferences.md#the-files-and-folders-tab). The system only considers a season folder to be a season folder if it follows the pattern ‘ nnnn'. The space between is optional and the number can be any length.

Click the `Auto ID All` button and TV Rename will try and identify the newly found shows. If the show is found the **Show** and **Source Code** columns will be populated. If a show isn’t being matched or is incorrectly identified highlight the row in question and use the `Edit` button to perform a manual search, and for a more in-depth interrogation you can use the `Visit TVDB` button which will launch a web browser targeting the shows page or `Open Folder` which will open the selected folder in Windows Explorer.

`Auto ID All` identifies each folder using, in this order:

1. a show ID in the folder name, if there is one (see below)
2. any NFO or XML file in the folder with a ‘tvdbid’ tag (Kodi format)
3. the show’s name, taken from the folder name

### Putting the show ID in the folder name

To make sure a folder is matched to the right show, add the show’s ID from TheTVDB, TMDB or TVmaze to the folder name. For example, each of these folders is identified as Silo:

* `Silo {tvdb-403245}`
* `Silo [tmdbid-125988]`
* `Silo tvmaze=38052`

Clicking `Remove` will remove the highlighted row from the New Shows list, however it will be re-detected in the next run of “Auto ID All”.

Clicking `Ignore` will add the folder to the list in the _**Ignore**_ tab and it will be ignored is subsequent scans.

## Bulk Add Movies

**Tools > Bulk Add Movies...** looks through your movie library folders for movie files that aren't in TV Rename yet, so you can add them to the **Movies** tab all at once.

### Choosing the folders

On the **Folders** tab, the **Monitor Folders** list shows your movie library folders. Click `Add` (or drag and drop folders onto the list) to add one, select a folder and click `Remove` (or press Delete) to take it off, or click `Open` (or double-click it) to open it in File Explorer. Changes made here change your movie library folders.

On the **Ignore** tab, the **Ignore Folders** list holds folders to skip when checking, with the same `Add`, `Remove` and `Open` buttons. This list is shared with Bulk Add Shows.

Click `Check >>` on either tab to start.

### Checking the folders

TV Rename opens the **Scan Results** tab and looks through each monitor folder and its subfolders, showing its progress as it goes. Click `Stop Scan` to stop early.

These are skipped:

* a monitor folder that is also one of your TV library folders
* folders on the Ignore list
* folders that already belong to a movie in TV Rename
* the Recycle Bin, if **Ignore Recycle Bin** is ticked
* folders with no video files in them, if **Only Include Folders containing Video files** is ticked

The last two options are on the [Scan Settings](../preferences.md#scan-settings) tab of **Options>Preferences**, in the **Bulk Add TV Shows from Library Folders** group, and apply to Bulk Add Movies as well.

{% hint style="warning" %}
If **Only Include Folders containing Video files** is not ticked, `Check >>` deletes any completely empty folder (one with no files and no subfolders) that it finds in your movie library folders.
{% endhint %}

### The New Movies list

Each video file found is listed under **New Movies**, with its **Folder**, and the **Movie**, **Year** and **Source Code** once the movie has been identified. You can also drag and drop a folder onto the list to check just that folder.

| Button                         | What it does                                                                                                                               |
| ------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------ |
| `Auto ID All`                  | Tries to identify every movie in the list that hasn't been identified yet.                                                                 |
| `Edit` (or double-click a row) | Opens a search so you can choose the right movie yourself.                                                                                 |
| `Remove` (or press Delete)     | Takes the selected rows off the list. They will be found again the next time you check.                                                    |
| `Ignore`                       | After you confirm, adds the selected folders to the Ignore Folders list and takes them off the list.                                       |
| `Visit TVDB`                   | Opens the selected movie's page on TheTVDB or TMDB, whichever it was identified from. It does nothing until the movie has been identified. |
| `Open Folder`                  | Opens the selected movie's folder in File Explorer.                                                                                        |

### Putting the movie ID in the file or folder name

To make sure a movie is matched to the right title, add its TMDB ID to the movie's file name or to its folder name. For example, either of these is identified as The Matrix (1999):

* a file named `The Matrix {tmdb-603}.mkv`
* a folder named `The Matrix {tmdb-603}`

Without an ID, `Auto ID All` searches for the movie by its name.

When you are ready, click `Add & Close`. TV Rename asks you to confirm, then adds every identified movie to the **Movies** tab. Movies that haven't been identified are not added.

Click `Close` to close the window without adding anything. If any movies have been identified, TV Rename asks you to confirm first.
