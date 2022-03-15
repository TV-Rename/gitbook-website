# Tools

## Tools

![The Tools Menu](https://www.tvrename.com/assets/images/tools/menu-01.png)Here you can find tools to update, manipulate and annihilate the data relating to your media library and [The TVDB](http://thetvdb.com) cache.

### Force Refresh All <a href="#force-refresh-all" id="force-refresh-all"></a>

![Force Refresh All](https://www.tvrename.com/assets/images/tools/force-refresh-all-01.png)If TV Rename’s representation of your media library is a mess then this is probably the tool for you.

After selecting the option from the menu you are presented with the alert window (shown).

**READ IT CAREFULLY AND PAY ATTENTION**. If you click `Yes` there’s no going back, all the locally stored information in TheTVDB’s cache will be **DELETED**.

[Return to Top](https://www.tvrename.com/manual/tools/)

### Background Download Now <a href="#background-download-now" id="background-download-now"></a>

**Background Download Now** forces an update from [The TVDB](http://thetvdb.com) to be downloaded. If _Options>Offline Operation_ is enabled you will be asked if you wish to “Ignore offline mode and download anyway” (Yes/No), if you select `Yes` the update will start.

[Return to Top](https://www.tvrename.com/manual/tools/)

### Bulk Add Shows <a href="#bulk-add-shows" id="bulk-add-shows"></a>

![The Tools>Bulk Add Shows window](https://www.tvrename.com/assets/images/tools/bulk-add-shows-02.png)This is where you tell TV Rename about the location(s) of your media library. Additionally you can check these locations for new folders unknown to TV Rename and quickly scan and add them to the _**My Shows**_ tab.

Before using this tool, check that your preferred renaming style is set in [_Options>Filename Template Editor_](https://www.tvrename.com/manual/options#filename-template-editor).

`Add` (or Drag-and-Drop) folders to the _**Folders:**_ tab. Click the `Check >>` button, and TV Rename will recursively search through the new folders looking for new TV shows. Once this is complete, if anything new is found, the _**Scan Results**_ tab will appear populated with the paths to any newly found shows, it will also identify the folder structure of the show (“Flat” - everything in one folder or “Folder per season”).

The system inspects each folder and if it contains any sub-folders that look like they are a season it assumes that they are structured in separate folders per season. TV Rename looks for any folders that start with any of the ‘season words’ entered in the preferences, with the default season word (again entered in preferences) and (if configured) any of the words used as season folder names for any of the shows in your library. The preferences for this function are specified [here](https://www.tvrename.com/manual/options/#the-files-and-folders-tab) and [here](https://www.tvrename.com/manual/options/#the-bulk--auto-add-tab). The system only considers a season folder to be a season folder if it follows the pattern ‘ nnnn'. The space between is optional and the number can be any length.

Click the `Auto ID All` button and TV Rename will try and identify the newly found shows using cached data from [The TVDB](http://thetvdb.com) . If the show is found the “Show” and “thetvdb code” columns will be populated. If a show isn’t being matched or is incorrectly identified highlight the row in question and use the `Edit` button to perform a manual search of [TheTVDB.com](http://thetvdb.com), and for a more in-depth interrogation you can use the `Visit TVDB` button which will launch a web browser targeting the shows page or `Open Folder` which will open the selected folder in Windows Explorer.

The `Auto ID All` function will use a combination of the show’s name as well as any NFO or XML files in the identified folder to help it try and guess the show being added. Any NFO or XML file with the ‘tvdbid’ tag will assist (Kodi format).

Clicking `Remove` will remove the highlighted row from the New Shows list, however it will be re-detected in the next run of “Auto ID All”.

Clicking `Ignore` will add the folder to the list in the _**Ignore**_ tab and it will be ignored is subsequent scans.

**Note:** A “glitch” in the design of the _**Ignore**_ tab means there is currently no obvious way to remove a folder from this list. The designers are aware of the problem and it will be fixed in the next release. Until then if you have a folder “stuck” in here that you want to be part of the library again, ask in the Main Forum and someone will help you fix it.

[Return to Top](https://www.tvrename.com/manual/tools/)

### Duplicate Episode Finder <a href="#duplicate-episode-finder" id="duplicate-episode-finder"></a>

![Duplicate Episode Finder](https://www.tvrename.com/assets/images/tools/duplicate-episode-finder-01.png)

The Duplicate Episode Finder will identify files in your library that contain two episodes of a show but do not have not had a merge rule applied…

Key things that might indicate this are: -

1. The two episodes on TVDB have the same air date.
2. The names of the episodes are similar.
3. One of the episodes has been matched to a file and the other has not.
4. The matched file is around twice the size of another for the same show.

If all (or some) of these criteria are met it’s probable that the file on disk actually represents both episodes.

Right clicking on an entry displays some options and the ability to auto-create the merge rule.
