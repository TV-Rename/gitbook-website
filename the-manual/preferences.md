---
description: Each of the tabs in “Preferences”, are discussed in detail below.
---

# Preferences

### General <a href="#the-general-tab" id="the-general-tab"></a>

![Preferences - the General tab](https://www.tvrename.com/assets/images/options/preferences-general-01.png)

The General Tab controls TV Renames’ Download and Scan behaviours.

_“X” days count as recent_ specifies how many days are listed for the “Aired in the last N days” section of the [_**When to watch**_](https://www.tvrename.com/manual/user#when-to-watch) tab.

_Default: **7 days**_

_Download up to “X” shows simultaneously from_ [_The TVDB_](http://thetvdb.com) sets the number of concurrent connections to TheTVDB API.

It can be set in the range 1 to 8.

_Default: **4**_

_Refresh entire series if “X” % of episodes are updated_ sets the point at which TV Rename refreshes the entire series data from [The TVDB](http://thetvdb.com) rather than just the episode data. This speeds up local data updates if major changes are made to a show on [The TVDB](http://thetvdb.com).

_Default: **20%**_

_Look for air date in filenames_, if ticked, provides a second method of identifying show episodes by looking for a date (in a number of formats) in the shows filename and comparing that against the air-date.

The supported date formats are:

“yyyy-MM-dd”, “dd-MM-yyyy”, “MM-dd-yyyy”, “yy-MM-dd”, “dd-MM-yy” and “MM-dd-yy”

And the “date separators” can be any of: - / . , and “ “ (a space)

_Default: **Un-ticked**_

The _Preferred language:_ drop-down sets the language for returned data when requesting information from TheTVDB API. TV Rename will request “English” If the selected language is not available.

The _Mode:_ drop-down can be set to “Production” or “Beta” and allows you to preview Beta functionality that is being worked on but not yet ready for the mainstream releases.

In “Production” mode the application looks and behaves as normal.

In “Beta” mode a new menu called Beta appears between Tools and Help in the menu bar which gives you access to preview upcoming additions and enhancements.

If you select “Beta”, TV Rename will offer you “Beta” and “RC” updates as well as the “Production” updates as and when they become available.

_Default: **Production**_

The _Share critical Logs to help defeat bugs_ option if ticked, gives TV Rename permission to copy some anonymous crash statistics to the [SolarWinds “papertrail”](https://papertrailapp.com) Log Management Tool to aid in debugging, as mentioned in the License Agreement. (See TV Rename’s _**Help>About**_.)

_Default: **Ticked**_

Looking at the _Scan Options…_

The “Scan Type” radio buttons tell TV Rename the type of scan to perform when searching for new shows.

| **Full**   | A full scan of all shows and seasons.                                                                |
| ---------- | ---------------------------------------------------------------------------------------------------- |
| **Recent** | A Scan of all the shows that have aired recently (as specified in _“X” days count as recent_ above). |
| **Quick**  | Scan the shows that have aired recently and have a missing episode in the library.                   |

| The scans also check the locations specified in [_**Options>Preferences - Search Folders**_](https://www.tvrename.com/manual/options#the-search-folders-tab) for any matching media files. |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |

Ticking _Scan on Startup_ tells TV Rename to perform the selected scan when the program starts. Ticking _Scheduled scan…_ will force a repeat scan every “X” hours.

_Scan Checks and Options_ has three major functions

_Rename Check_ will tell TV Rename to correct found episode names to the found content from [The TVDB](http://thetvdb.com).

_Missing Check_ will tell TV Rename to check for missing episodes. Additionally this option must be ticked to enable changes in the [_**Torrents / NZB**_](https://www.tvrename.com/manual/options#the-torrents--nzb-tab) tab.

_Move Files within Library to Keep it Tidy_ will do just that, if files have been directly added to or misplaced in the library enabling this setting will tidy stuff to the correct names and places.

| _Defaults:_                               |                                |
| ----------------------------------------- | ------------------------------ |
| Scan Type                                 | _**Full**_                     |
| Scan on Startup                           | _**Un-ticked**_                |
| Scheduled scan every                      | _**Un-ticked**_ - _**1 hour**_ |
| “Scan” checks and actions                 |                                |
| Rename Check                              | _**Ticked**_                   |
|   Prevent move of flies                   | _**Un-ticked**_                |
| Missing Check                             | _**Ticked**_                   |
|   Ignore Episodes Previously Seen         | _**Un-ticked**_                |
| Move Files within Library to Keep it Tidy | _**Ticked**_                   |

### Display <a href="#the-display-tab" id="the-display-tab"></a>

![Preferences - The Display tab](https://www.tvrename.com/assets/images/options/preferences-display-01.png)

The Display tab allows you to change how TV Rename looks. Its effects are purely visual, it does not change functionality.

_Double-click in When to Watch does:_ Controls the double-click action in the [_**When to watch**_](https://www.tvrename.com/manual/user#when-to-watch) tab. Its options are _Search_ or _Scan_.

_Default: **Search**_

The _Startup Tab:_ selects which tab you wish open when TV Rename loads. _**My Shows**_, _**Search**_ or _**When to Watch**_.

_Default: **My Shows**_

The _Show Notification Area_ and _Show in Taskbar_ interact, one of them **must** be ticked. If you try to un-tick both the option you are modifying clears, but the other one automatically sets.

If _Show in Taskbar_ is selected TV Rename’s icon appears in the Windows taskbar.\
If _Show Notification Area_ is selected TV Rename’s icon appears in the System Tray. Right-clicking it will show an “Upcoming Shows” list, and double clicking restores the main window.\
Both boxes can be ticked, in which case you get both functionalities.

| _Defaults:_            |                 |
| ---------------------- | --------------- |
| Show Notification Area | _**Un-ticked**_ |
| Show in Taskbar        | _**Ticked**_    |

_Show episode pictures in episode guides_ Does what-it-says-on-the-tin, if ticked, screen grabs from show episodes are displayed with the episode description in the _**My Shows**_ tab. If un-ticked only the episode description is displayed.

_Default: **Ticked**_

_Hide Spoilers in My Shows_ hides the display of summaries of yet to be broadcast episodes (with a suitable message) in the _**My Shows**_ tab

_Default: **Un-ticked**_

_Hide Spoilers in When To Watch_ hides the display of summaries of yet to be broadcast episodes (with a suitable message) in the _**When to watch**_ tab

_Default:_ _**Un-ticked**_

Bearing in mind that we are in the _**Display**_ tab, the next option _Move “The” to the end of show names_ only affects the display of the show list in the _My Shows_ tab and **not** the contents of the library.

If ticked show names starting with “The” will be displayed and sorted with “, The” at the end. For example, “The Hollow Crown” would be listed as “Hollow Crown, The” and displayed with the other shows starting with “H”

_Default:_ _**Un-ticked**_

_Automatically select show and season in My Shows_ If ticked this works for both the _**When to watch**_ and _**Scan**_ tabs. If an item is selected in either of these tabs the _**My Shows**_ tab is automatically updated to highlight the indicated show and season.

_Default:_ _**Ticked**_

The _Season Name_ and _Leading 0 on Season numbers_ options allow you control of the season text and number display in the _**My Shows**_ tab.

Ticking the _Show Basic Shows Detail_ box will force TV Rename to revert to the older style display of data in the right hand panel of the _**My Shows**_ tab, which may behave better on smaller screens, slower pc’s and slower internet connections.

_Default:_ _**Un-ticked**_

If you have a large catalogue of TV Shows that you want to keep on the system, the _**My Shows**_ tab can become somewhat cluttered. _Show Colouring_ can help by applying some order…

With _Show Colouring_ you can change the color of the text on the left hand pane of the _**My Shows**_ tab depending on the status of the show or the show season.

To create a record:-

* Expand the _“Status:”_ drop-down at the bottom of the window and select the status you wish to match from the list.
* Select a color to associate with the status by either entering a web-safe color name or code in the _“Text Color:”_ box or clicking `Select Colour` and choosing from the pallet.
* Click the `Add` button and your new entry will appear the box above.

For example: to make finished shows less obtrusive in _**My Shows**_ expand the _“Status:”_ drop-down and select _“Show Status: Ended”_, in the _“Text Color:”_ box type _“#808080”_ and click `Add`. Back in the _**My Shows**_ tab; text for shows that have finished will be light grey and less obtrusive.

If you wish to remove a rule from the list just select it and click `Remove`.

### Library Folders <a href="#the-library-folders-tab" id="the-library-folders-tab"></a>

![Preferences - the Library Folders tab](https://www.tvrename.com/assets/images/options/preferences-library-folders-01.png)The Library Folders tab is used to tell TV Rename about the location(s) of your Media Library - viz where to look for TV Show episode files **AFTER** they have been processed.

To tell TV Rename about your library simply use the `Add` button to browse to a folder that is a “Base” folder of your Media Library. and click `OK`.

You can also highlight a path in the list and use the `Remove` button to remove it, and highlight a path in the list and use `Open` to check its contents in a File Explorer window.

“Base” folder refers to a path on your system that corresponds to the location of your media files.

```
  D:\                                      nas-1
  └─ media                                 └─ media
     └─ Video                                 └─ Video
        └─ TV Shows                              └─ TV Shows
           ├─ Show A                                ├─ Show C
           │  ├─ Season 1                           │  ├─ Season 1
           │  │  ├─ Episode 1                       │  │  ├─ Episode 1
           │  │  └─ Episode 2                       │  │  └─ Episode 2
           │  └─ Season 2                           │  └─ Season 2
           │     ├─ Episode 1                       │     ├─ Episode 1
           │     └─ Episode 2                       │     └─ Episode 2
           └─ Show B                                └─ Show D
              ├─ Season 1                              ├─ Season 1
              │  ├─ Episode 1                          │  ├─ Episode 1
              │  └─ Episode 2                          │  └─ Episode 2
              └─ Season 2                              └─ Season 2
                 ├─ Episode 1                             ├─ Episode 1
                 └─ Episode 2                             └─ Episode 2
```

For the folder structure illustrated (above left) the base folder would be “D:\media\Video\TV Shows”.

This could also be a UNC path (above right) to a device for example: “\\\nas-1\media\Video\TV Shows”.

_Additional Scan Options_ allow manipulation of the Medial Library contents.

_Update files and folders with air date_, if ticked, will modify the time stamp of files and folders in the Media Library to match the original air date of the episode being copied or moved.

_Default: **Un-ticked**_

**NOTE:** If you use a NAS device as your media library and it is Linux based it has an epoch date of 01/01/1970 00:00. Files cannot have a date/time-stamp earlier than this. If you have any TV Show episodes whose original release date was earlier and you have the _Update files and folders with air date_ box ticked they will be set to 01/01/1970 00:00.

_Automatically create merge rules for merged library episodes_ simply looks at the filename. If it matches one of the multi-episode regexes (see [**Options>Filename Processors**](https://www.tvrename.com/manual/options#filename-processors)) it will create the appropriate merge rule.

If your library contains:

```
  ├─ My Favourite Show
  │   ├─ Season 1
  │   │  ├─ My Favourite Show - S01E01 - A Great Episode
  │   │  ├─ My Favourite Show - S01E02E03 - A Great Double Episode
  │   │  ├─ My Favourite Show - S01E05 - Another Great Episode
  │   │  ├─...
```

If disabled, E03 and E04 would be shown as “missing” (and E02E03 would be renamed as E02)

If enabled a new merge rule for S01E02E03 would be created and and only episode S01E04 would be shown as missing

_Default: **Un-ticked**_

_Automatically create missing folders_ simply gives TV Rename permission to create missing folders in the library without prompting.

_Default: **Un-ticked**_

_Bulk Add_ can be run from the TV Rename menu (see [**Tools>Bulk Add Shows**](https://www.tvrename.com/manual/tools#bulk-add-shows)) or as part of each scan.

The _Do Bulk Add as part of scan_ tick box enables or disables this option.

_Default: **Un-ticked**_

Looking at the _Bulk Add Shows from Library Folders_ section, three options are available.

The first two work as “junk filters”.

_Only Include Folders containing Video Files_ if ticked restricts the “Bulk Add” scan to only include folders with video files.

_Default:_ _**Un-ticked**_

_Ignore Recycle Bin_ tells the “Bulk Add” scan to exclude the (Windows) Recycle Bin even if it contains video files.

_Default:_ _**Un-ticked**_

Finally, _Force to Use Season Words from Settings only_ tells the “Bulk Add” scan to just use the words entered in the associated text box when scanning to decide whether the series has a flat structure or a ‘folder by season’ structure.

| _Defaults:_                                    |                                              |
| ---------------------------------------------- | -------------------------------------------- |
| _Force to Use Season Words from Settings only_ | _**Un-ticked**_                              |
| _Season Search Terms_                          | _**Season;Series;Saison;Temporada;Seizoen**_ |

The Last two preferences allow you to set the text for the “Specials” and “Season” folders - useful if you speak “English as a second language”.

The _Specials folder name:_ text box allows you to modify the name used when creating a “Specials” folder for a show.

It is common practice for specials to be labeled as part of “Season 0” so for example: special 3 of “Battlestar Galactica” would be labeled “Battlestar Galactica - S00E03 - The Story So Far” and stored (by default) in the “Specials” folder.

_Default:_ _**Specials**_

Similarly, the _Season folder format:_ text box allows you to customise the name used when creating a “Season” in your media library. ({Season} is replaced by the season number.)

_Default:_ _**Season {Season}**_

An entry of “Season {Season:2}” here will result in seasons using 2 digit numbers -

_Season 01, Season 02 etc._

The `Tags` button will pop up a list of the tags that TV Rename will recognise in the _Season folder format:_ text box.

An entry of “Season {Season:2}” here will result in seasons using 2 digit numbers -

_Season 01, Season 02 etc._

The `Tags` button will pop up a list of the tags that TV Rename will recognise in the _Season folder format:_ text box.

[Return to Top](https://www.tvrename.com/manual/options/)

### The Files and Folders Tab <a href="#the-files-and-folders-tab" id="the-files-and-folders-tab"></a>

![Preferences - The Files and Folders tab](https://www.tvrename.com/assets/images/options/preferences-files-folders-01.png)The Files and Folders tab is used to manipulate how TV Rename copies or moves files from the “[Search Folders](https://www.tvrename.com/manual/options#the-search-folders-tab)” to the “[Library Folders](https://www.tvrename.com/manual/options#the-library-folders-tab)”.

The _Filename Replacements_ grid controls the replacement of illegal (Windows) characters in filenames.

If a filename contains a character that isn’t supported in Windows the grid is checked (row by row) to discover what to use instead of the problem character.

The grid can be edited using the `Add` and `Remove` buttons and case sensitivity can be turned off for specific rows using the _Case Ins._ check boxes.

_Video Extensions:_ tells TV Rename what to match when looking for video files. The entries should be semicolon delimited, not contain spaces and include the “.” preceding the extension.

_Default: **.avi;.mpg;.mpeg;.mkv;.mp4;.wmv;.divx;.ogm;.qt;.rm**_

_Other Extensions:_ follows the same rules as _Video Extensions_ but the file extensions specified are for related files rather than actual videos. Files with these extensions will be renamed when scanning through the library.

| _Defaults:_ |                                                                                                                                                                                                                                |
| ----------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| _**.srt**_  | Subtitles in text format.                                                                                                                                                                                                      |
| _**.nfo**_  | An XML style file that contains information about the video, such as a title, summary, list of actors, year of production etc. This information is often used by media players to provide a more immersive viewing experience. |
| _**.txt**_  | Text files can be any text but quite often, if the base name of the text file is the same as that of the video file, they contain subtitles in text format.                                                                    |
| _**.tbn**_  | A KODI/XBMC specific jpeg.                                                                                                                                                                                                     |

This second list deals with files you’d like to copy/move when TV Rename finds a missing episode in the search folders. The extensions may be different from those used in the library list because (for example) you may not want .nfo files not to be copied from the search folders because TV Rename creates them but once created then you’ll want them to be renamed with the source file(s).

It is common practice for files related to a specific video to have the same base name.

For example: BigBuckBunny.avi, BigBuckBunny.sub and BigBuckBunny.nfo. This helps keep them organised.

TV Rename knows this, hence the _Copy/Move file with same base name as video_ tick-box which gives you the ability to turn this functionality on or off.

_Default:_ _**Ticked**_

The _Do_ drop-down and text box underneath provide a degree of granularity to this function.

If _Do_ is set to **All** the extensions listed in the text box are ignored.

If _Do_ is set to **All but these** the extensions listed in the text box are treated as an exclude list.

If _Do_ is set to **Just** the extensions listed in the text box are treated as an include list.

| _Defaults_        |                           |
| ----------------- | ------------------------- |
| _Do_ drop down    | _**All**_                 |
| Text box contents | _**.srt;.nfo;.txt;.tbn**_ |

_Ignore “sample” videos_ and _Make all filenames lower case_ tick boxes need no further explanation.

The _Use name of Library Folder…_ option extends the search for a show name to include the containing library folder name, negating the need for the show name to be present in the filename.

The _**Subtitles**_ section is used to tell TV Rename how to handle subtitle files in your collection.

The Retain Language Specific Subtitles tick box (when ticked) tells TV Rename to retain subtitle files containing two or three letter language codes. For example: -

Video S01E01.en.srt

Subtitles must be of the form \*.language.extension, where language is 2 or 3 characters.

_Default:_ _**ticked**_

Subtitle files come in a number of guises of which one of the most common is a .sub file. These are text files structured in a way that media players can establish the start time, finish time and content of a subtitle and display it. Quite often sources for these files give them a .txt extension, for example: BigBuckBunny.txt. Ticking the “Rename .txt to .sub” option will tell TV Rename to rename these files when copied or moved.

_Default:_ _**Un-ticked**_

The _Subtitle extensions:_ text box lists the commonly used subtitle extensions.

_Default:_ _**.srt;.sub;.sbv;.idx**_

### Search Folders <a href="#the-search-folders-tab" id="the-search-folders-tab"></a>

![Preferences - the Search Folders tab](https://www.tvrename.com/assets/images/options/preferences-search-folders-01.png)__

_Search Folders_ tell TV Rename where to look for TV Show episode files **BEFORE** they are processed and copied or moved to the media library.

The functionality of the first five tick boxes requires little explanation.

_Look in “Search Folders” for missing files_ enables the search functionality when ticked.

_Copy files, don’t move_, if ticked will tell TV Rename to copy and files to the media library leaving the originals intact.

_Automatically create merge rules based on files in Search Folders_ is similar to the functionality found in [**Library Folders**](https://www.tvrename.com/manual/options#the-library-folders-tab) except the appropriate record is created before moving/copying the file rather than after.

_Monitor folders for changes_, if ticked, will trigger a scan if Windows detects a change in any of the source folders.

_Copy future dated episodes found in Search Folders_ handles files that are found to exist before their release date.

| _Defaults_ |                                                                     |                 |
| ---------- | ------------------------------------------------------------------- | --------------- |
|            | _Look in “Search Folders” for missing files_                        | _**Ticked**_    |
|            |   _Copy files, don’t move_                                          | _**Un-ticked**_ |
|            | _Automatically create merge rules based on files in Search Folders_ | _**Un-ticked**_ |
|            | _Monitor folders for changes_                                       | _**Un-ticked**_ |
|            | _Copy future dated episodes found in Search Folders_                | _**Un-ticked**_ |

The _Search Folders_ window allows you to add, delete or check the paths to your search folders.

Logical entries in here would be your downloads folder (if you download TV show episodes from the internet) or maybe your desktop (if you rip TV show episodes from DVD or Blu-ray). Or both!

Three buttons are available. `Add` opens an explorer style window so you can browse to the folder location you wish to add and click `OK`, `Remove` removes a highlighted row from the panel and `Open` opens an explorer window targeting the row highlighted in the panel.

The _Auto Add:_ section comes in to play when the **Preferences>Search Folders - Notify when new shows are found** option is ticked.

The _Movie Terms:_ text box helps TV Rename identify “types” of video file.

_Default:_ _**dvdrip;camrip;screener;dvdscr;r5;bluray**_

The _Ignore Suffixes:_ text box tells TV Rename to ignore the specified suffixes.

_Default:_ _**1080p;720p**_

_Update episodes when higher quality ones found:_ tells TV\&nbsp:;Rename to replace files in the video library with higher quality versionbs if they are found.

| _Default:_ _**Un-ticked**_ |
| -------------------------- |

The final two options act as “helpers” for TV Rename when replacing videos that already exist in the library.

The _Priority override terms:_ text box defines the “hints” used to determine if a video has been improved at source.

_Default:_ _**PROPER;REPACK;RERIP**_ (Note the semicolon delimiter).

_Consider a file better if it is **X%** higher resolution/longer_ tells TV Rename to replace an existing library file if the newly found version is higher resolution and/or longer.

_Default:_ _**10%**_

### Folder Deleting <a href="#the-folder-deleting-tab" id="the-folder-deleting-tab"></a>

![Preferences - the Folder Delete tab](https://www.tvrename.com/assets/images/options/preferences-folder-del-01.png)This tab is all about TV Rename tidying up after itself.

When downloading video from the internet its quite common to get .nfo files, screen grabs, sample video, text-art files and the like bundled with the download.

TV Rename automatically takes care of the video file and any others you media play may require, renaming them and copying or moving them to your media library.

The settings in this tab take care of the rest.

The flow through this tab is pretty self explanatory, start by ticking the _Delete empty folders…_ tick box to enable the action.

The other settings are fairly obvious, tick the boxes and modify the text as required. It should be noted that _Ignore any files with these words…_ also includes folders.

If you use the copy option to update your library then ticking the _Clean up already copied…_ box will delete the source files after the copy is complete.

_Default:_ _**All functionality disabled**_

### Media Centers <a href="#the-media-centers-tab" id="the-media-centers-tab"></a>

![Preferences - the Media Centre tab](https://www.tvrename.com/assets/images/options/preferences-media-center-01.png)Here you can tell TV Rename about your media player (and hence, any additional files you may need to download).

The tick box options in each group should already be familiar to you if you use that particular media player.

The `Presets` button (bottom right) allows you to quickly apply all the relevant presets for the chosen media player.

### RSS / JSON Search <a href="#the-rss--json-search-tab" id="the-rss--json-search-tab"></a>

![Preferences - The RSS/JSON Search Tab](https://www.tvrename.com/assets/images/options/preferences-rss-json-search-01.png)RSS and JSON Searches give TV Rename additional methods of looking for missing files in your media library, providing URLs for the torrent handlers to use.

**RSS Search**

The _Search RSS for missing files_ tick box enables the RSS search mechanism when ticked.

_Default: **Un-ticked**_

When enabled the “RSS Search” pane is activated.

The _Only on manual scans_ further restricts the RSS Search, stopping it from running on automatic scans.

_Default: **Ticked**_

The _Preferred Terms:_ text box acts as a filter on the RSS Search and contains a semicolon delimited list. There must be a match in the RSS feed to return a search result. The default entry will only find RSS feed results that contain 720p or 1080p in the video names.

_Default: **720p;1080p**_

_The Torrent RSS URLs:_ can be any suitable RSS-feeds provided by indexers or public RSS websites and are used to search for missing files.

`Add` and `Remove` allow you to add and remove feeds, and `Open` presents the highlighted feed in a web browser.

**JSON Search**

The JSON Search is broadly similar.

It downloads information from the web and searches for useful content.

**NOTE:** Please be aware that JSON Search is currently tightly tied to the EZTV API, and may not work in some countries due to ISP filtering.

Basically the JSON Search:

1. Takes the URL from the settings.
2. Appends the IMDB id.
3. Downloads the data.
4. Goes to the node indicated by the “root Note”.
5. Iterates across items in that node looking for tags with “Filename Token” and “URL token”.
6. If the filename token looks like it is something useful it downloads the URL token.

| _Defaults_ |                                 |                 |
| ---------- | ------------------------------- | --------------- |
|            | _Search JSON for missing files_ | _**Un-ticked**_ |
|            | _Only on manual scans_          | _**Ticked**_    |

**If things go wrong…**

Ticking the “Detailed logging” box will greatly increase the log detail around either the RSS or JSON searches providing lots of detail - useful ifyou are having trouble setting up either of the searches.

It is recommended that you only use this option if you need to. When ticked the size of the log file will grow very quickly.

### Torrents / NZB <a href="#the-torrents--nzb-tab" id="the-torrents--nzb-tab"></a>

![Preferences - the Torrents / NZB tab](https://www.tvrename.com/assets/images/options/preferences-torrent-nzb-01.png)

TV Rename can check SABnzbd µTorrent and qBittorent queues and uses the information on this tab to know where to look for more information.

**NOTE:** to activate this tab the _Missing Check_ box on the [_**General**_](https://www.tvrename.com/manual/options#the-general-tab) tab **MUST** be ticked.

Both the “Host Port” and “API Key” are required to use this functionality in SABnzbd.

If you use µTorrent, TV Rename needs to know the “Application” and “resume.dat” paths, (they can be found with the `Browse` buttons) so it can detect if files are queued or in the process of being downloaded.

TV Rename uses the qBittorrent web interface to interrogate its status so you must turn on the Web UI in qBittorrent and tell it to “Bypass authentication for clients on localhost” if you wish to use this client. In addition TV Rename needs to know the host name and port for the interface so it can communicate with the client (defaults shown).

| _Defaults_ |                         |                 |
| ---------- | ----------------------- | --------------- |
|            | Check SABnzdb queue     | _**Un-ticked**_ |
|            | Check µTorrent queue    | _**Un-ticked**_ |
|            | Check qBittorrent queue | _**Un-ticked**_ |

### Automatic Export <a href="#the-automatic-export-tab" id="the-automatic-export-tab"></a>

![Preferences - the Automatic Export tab](https://www.tvrename.com/assets/images/options/preferences-auto-export-01.png)Ticking the “RSS” box in the “When to watch” section of the panel will save a RSS-reader compatible XML file to the location you specify (by typing or browsing). This file can then be read by something like XBOX Media Center, or a Windows RSS App.

Ticking the “XML” box in the “When to watch” section of the panel will save a standard XML file to the location you specify (by typing or browsing).

Ticking the “iCal” box in the “When to watch” section of the panel will save an open format Internet Calendar ICS file (not to be confused with Apple Calendar) to the location of you specify (by typing or browsing).

You can limit how many days or shows are written to the file. The files are updated whenever the “When to watch” tab is manually or automatically refreshed.

Ticking the “XML” box in the “Missing” section of the panel will save a standard XML file containing the missing episodes detected during a scan to the location you specify (by typing or browsing).

Similarly, ticking the “CSV” box in the “Missing” section of the panel will save a standard CSV file containing the missing episodes detected during a scan to the location you specify (by typing or browsing).

Ticking the “TXT” box in the “All Shows” section of the panel will save a TXT file whenever a show is added, edited or deleted from TV Rename. It also gets updated when `Auto ID All` in the _Scan Results_ tab of **Tools>Folder Monitor** is clicked.

Similarly, ticking the “HTML” box in the “All Shows” section of the panel will save a web browser viewable HTML file containing the show summary for each show in your library (complete with images and other details) whenever a show is added, edited or deleted from TV Rename. It also gets updated when `Auto ID All` in the _Scan Results_ tab of **Tools>Folder Monitor** is clicked.

Ticking the “XML” box in the “Renaming” section of the panel will create an XML file in the path specified containing the rename data.

Ticking the “XML” box in the “Finding and Organising” section of the panel will create an XML file in the path specified containing the found file data.

The “Recent Playlist” section of the tab tells TV Rename to export a playlist of all the episodes found in the “Aired in last X days” section on the _**When to watch**_ tab in the specified format to the specified file and location.

_Default:_ _**All un-ticked**_
