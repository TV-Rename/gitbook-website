# Bulk Add

## Bulk Add Shows <a href="#bulk-add-shows" id="bulk-add-shows"></a>

![The Tools>Bulk Add Shows window](https://www.tvrename.com/assets/images/tools/bulk-add-shows-02.png)

This is where you tell TV Rename about the location(s) of your media library. Additionally you can check these locations for new folders unknown to TV Rename and quickly scan and add them to the _**My Shows**_ tab.

Before using this tool, check that your preferred renaming style is set in [_Options>Filename Template Editor_](https://www.tvrename.com/manual/options#filename-template-editor).

`Add` (or Drag-and-Drop) folders to the _**Folders:**_ tab. Click the `Check >>` button, and TV Rename will recursively search through the new folders looking for new TV shows. Once this is complete, if anything new is found, the _**Scan Results**_ tab will appear populated with the paths to any newly found shows, it will also identify the folder structure of the show (“Flat” - everything in one folder or “Folder per season”).

The system inspects each folder and if it contains any sub-folders that look like they are a season it assumes that they are structured in separate folders per season. TV Rename looks for any folders that start with any of the ‘season words’ entered in the preferences, with the default season word (again entered in preferences) and (if configured) any of the words used as season folder names for any of the shows in your library. The preferences for this function are specified [here](https://www.tvrename.com/manual/options/#the-files-and-folders-tab) and [here](https://www.tvrename.com/manual/options/#the-bulk--auto-add-tab). The system only considers a season folder to be a season folder if it follows the pattern ‘ nnnn'. The space between is optional and the number can be any length.

Click the `Auto ID All` button and TV Rename will try and identify the newly found shows using cached data from [The TVDB](http://thetvdb.com) . If the show is found the “Show” and “thetvdb code” columns will be populated. If a show isn’t being matched or is incorrectly identified highlight the row in question and use the `Edit` button to perform a manual search of [TheTVDB.com](http://thetvdb.com), and for a more in-depth interrogation you can use the `Visit TVDB` button which will launch a web browser targeting the shows page or `Open Folder` which will open the selected folder in Windows Explorer.

The `Auto ID All` function will use a combination of the show’s name as well as any NFO or XML files in the identified folder to help it try and guess the show being added. Any NFO or XML file with the ‘tvdbid’ tag will assist (Kodi format).

Clicking `Remove` will remove the highlighted row from the New Shows list, however it will be re-detected in the next run of “Auto ID All”.

Clicking `Ignore` will add the folder to the list in the _**Ignore**_ tab and it will be ignored is subsequent scans.

{% hint style="info" %}
**Note:** A “glitch” in the design of the _**Ignore**_ tab means there is currently no obvious way to remove a folder from this list. The designers are aware of the problem and it will be fixed in the next release. Until then if you have a folder “stuck” in here that you want to be part of the library again, ask in the Main Forum and someone will help you fix it.
{% endhint %}

## Bulk Add Movies <a href="#duplicate-episode-finder" id="duplicate-episode-finder"></a>
