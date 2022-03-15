---
description: Adding Shows
---

# Features

### Adding Shows <a href="#adding-shows" id="adding-shows"></a>

#### Functionality <a href="#functionality" id="functionality"></a>

TV Rename will track many TV Shows in your library. These can be added in 3 key ways:

* _Manually_ – Added manually by entering the name into the ‘Add Show’ screen from the main ‘My Shows’ tab
* _Bulk Add_ – TV Rename can scan through some specified folders (Monitor Folders) via the ‘Bulk Add’ tool. It will display a list of shows that are not already in the library and allow them to be added en-masse.
* _Automated_ – TV Rename can be setup to look at files in the download folder (Search Folders) and (if it can’t find an appropriate show in the library) offer the user some suggestions about which series/show to add to the library.

**Manual Addition**

Manual addition is the simplest way of adding shows into the library. You can enter (and search for) the show by name or for more precise addition enter a TVDB Id. All the options about the show can be edited, but they key ones to add are:

* Directory location to store the location of the files for the series
* Time zone for the series (this is not available from TVDB, so must be entered manually)

**Bulk Addition**

TV Rename can search through your library of existing (organised) files to find shows that are not in the library. This is initiated from the menu bar, with config options are in the preferences under ‘Bulk/Auto Add’. It can be made to ignore folders with no video files and recycle bin from the configuration options. If specific folders should be ignored, then they can be from the within the tools. (specify ignore folders)

**Automated Addition**

TV Rename can look at ‘spare’ files in the ‘download’/Search folders;

* If it cannot find a home for them then
* It tries to find the series on TVDB and asks the user for clarification via a streamlined add dialog.
* Once accepted, TVR automatically adds the show.
* If auto folder creation is on, then the folders get created in the library automatically and the appropriate files copied in.

#### Further Information <a href="#further-information" id="further-information"></a>

This function can be turned on using the tick box in [**Options>Preferences>Bulk / Auto Add - Notify when new shows are found**](https://www.tvrename.com/manual/options#the-bulk--auto-add-tab). There are options here to help modify filenames into show names by ignoring certain terms and by ignoring files altogether with specific terms in the filename.

### Scanning <a href="#scanning" id="scanning"></a>

#### Functionality <a href="#functionality-1" id="functionality-1"></a>

**Scan Types**

There are 4 types of scan:

* _Single Show_ – A single show can be scanned manually.
* _Quick Scan_ - A ‘clever’ scan that looks in the download directory for shows to scan. It also scans missing episodes from the recent list.
* _Recent Scan_ – A scan that looks at all shows that have had an episode aired in the last few days. The number of days can be specified in the preferences.
* _Full Scan_ – Scans all shows that are set to be scanned.

**Triggering Scans**

These can be triggered in several ways:

* On Startup
* Via Command Line
* Periodic (Automated)
* When download/search folder/file changes
* Manually

#### Further Information <a href="#further-information-1" id="further-information-1"></a>

* Configuration options are detailed in [**Options>Preferences>Scan Options**](https://www.tvrename.com/manual/options#the-scan-options-tab)
* Further explanation can be found [**here**](https://www.tvrename.com/manual/user#scan).

#### Future Ideas <a href="#future-ideas" id="future-ideas"></a>

* To incorporate a ‘Bulk add’ as part of the scan and use the new ‘Quick Add’ Dialog to quickly add missing shows.

### Finding <a href="#finding" id="finding"></a>

#### Functionality <a href="#functionality-2" id="functionality-2"></a>

Once a scan is complete, TV Rename will identify files to move/copy/rename and additional files to download/create. For episodes that are still missing, TV Rename will try and find them for you.

#### Types <a href="#types" id="types"></a>

There are 6 places it could search:

* _File System_ – If found it will remove the episode from the missing list and move the file into the correct place.
* _RSS Feed for torrent links_, _JSON Web page for torrent links_ – If found then it will download the torrent file. (via uTorrent or qBittorrent) See [**The RSS/JSON Search Tab**](https://www.tvrename.com/manual/options/#the-rss--json-search-tab) for more information about configuration.
* _SABnzbd_, _uTorrent_, _qBittorrent_ – If found it will mark it as downloading so you know not to try and find the item again. See [**The Torrents/NZB Tab**](https://www.tvrename.com/manual/options/#the-torrents--nzb-tab) for more informaiton.

#### How to write a Regex for TV Rename <a href="#how-to-write-a-regex-for-tv-rename" id="how-to-write-a-regex-for-tv-rename"></a>

Firstly, get acquainted with what a regular expression is - these sites will help:

* [**regexone.com**](https://regexone.com)
* [**www.regular-expressions.info**](https://www.regular-expressions.info)
* [**regexr.com**](https://regexr.com)
* [**regex101.com**](https://regex101.com)
* [**www.rexegg.com**](http://www.rexegg.com/regex-quickstart.html)

Once you understand Regular Expressions and [**‘Named Groups’**](https://www.regular-expressions.info/named.html) in particular then all you need to know is that TV Rename looks for 3 named groups:

* _S_ – The number series the file relates to.
* _E_ – The Episode number the file relates to.
* _F_ – (optional) If specified and if it matches then this is the max episode number that the file matches. It is used for instances when a file matches multiple episodes.

For Example: ‘S01E01-03’ would indicate that the file represents Series 1 and is episodes 1-3. In this case S=1, E=1 and F=3.

#### Finding Rules <a href="#finding-rules" id="finding-rules"></a>

Note that if a file matches multiple missing files, or multiple files match one missing episode no action is taken. TV Rename will raise a warning in the log files and allow the user to manually link the file to the missing episode.

### Further Information <a href="#further-information-2" id="further-information-2"></a>

Further information can be found [**here**](https://www.tvrename.com/manual/options/#filename-processors) and [**here**](https://www.tvrename.com/manual/options/#the-%C2%B5torrent--nzb-tab).

### Future Ideas <a href="#future-ideas-1" id="future-ideas-1"></a>

There is a related “Feature Suggestion” on our Idea Wall [**here**](http://ideas.theideawall.com/TVRename/Forum/TopicDetails/e6663947-906a-4a91-95ae-e45a91c6efb0).

### Organising <a href="#organising" id="organising"></a>

While the main objective of TV Rename is to rename and move/copy files into the appropriate locations in the library, there are many other things it can do at the same time:

#### Keep Files Together <a href="#keep-files-together" id="keep-files-together"></a>

The system will keep files that share the same name together, renaming them all as one. This keeps related files (images, information, metadata) joined together. The system can also be configured to keep language specific files together for when you have subtitles in multiple languages.

**Further Information**

Further information can be found [**here**](https://www.tvrename.com/manual/options/#the-files-and-folders-tab).

#### File Update Timestamp <a href="#file-update-timestamp" id="file-update-timestamp"></a>

The system can also be requested to update the ‘last updated’ dates to match the air-dates. This aims to help DNLA systems, but be wary if you are using a Linux based system such as a NAS for your media library. Linux has an inception date of 01/01/1970 and does not support earlier dates.

#### DVD vs Aired Order <a href="#dvd-vs-aired-order" id="dvd-vs-aired-order"></a>

TV Rename can order a series in 2 ways at present:

* Aired Season Order
* DVD Season Order

To show how these are different take a look at Futurama on [The TVDB](http://thetvdb.com/series/futurama) and you can see that the episode order on DVD does not match the Aired order.

**Future Ideas**

There are a few ideas on the ideas wall to allow the ordering to be adjusted further to account for shows such as Mythbusters and American Dad. In both these cases the order that users want to organise the files does not match either the Aired or the DVD order

* [**Allow reorganising season numbers**](http://ideas.theideawall.com/TVRename/Forum/TopicDetails/1c0aeb70-98ae-4937-9de3-8243ca61fcf2)
* [**Allow offset for episode numbers**](http://ideas.theideawall.com/TVRename/Forum/TopicDetails/ccf342c0-94b0-42f2-a0ba-a7cda261b2fa)

#### Media Centres <a href="#media-centres" id="media-centres"></a>

In addition to renaming and moving files the system can also download/create files for various media players:

* Kodi
* Mede8er
* pyTivo
* WD TV Live Media Player
* others

In each case then the following types of files can be downloaded

* Fanarts, banners and posters
* Episode screenshots
* XML/Text files to explain details about the show/series/episodes

**Further Information**

Further information can be found [**here**](https://www.tvrename.com/manual/options/#the-media-center-tab).

**Future Ideas**

There are plans to add support for other media centres and provide additional information by analysing the video files in more detail:

* [**Get the codec, size etc and use to show images in the show guide**](http://ideas.theideawall.com/TVRename/Forum/TopicDetails/861a5956-e5d4-466e-baf7-1f137b7c5855).
* [**AtomicParsley/MKVPropEdit support**](http://ideas.theideawall.com/TVRename/Forum/TopicDetails/2934aef8-4dfe-4503-a995-81b95542a6bf)
* [**Support for additional Media Centres**](http://ideas.theideawall.com/TVRename/Forum/TopicDetails/74204b8a-836a-4a6e-997d-09ea4fe39362)

### Automating <a href="#automating" id="automating"></a>

Functionality TV Rename aims to do as much as it can to automate the storage of media files. To make the process as automated as possible it can:

* _Auto Add shows_ – see ‘Automated Addition’ above.
* _Auto folder creation_ – TV Rename can be setup via preferences [(**here**)](https://www.tvrename.com/manual/options#the-scan-options-tab) to automatically create folders for shows and series. This will create based on the defaults.
* _Auto folder & file deletion_ – TV Rename can identify files and folders that can be removed and then get rid of them.
  * _‘Delete Empty Folders after moving Files’_ - Review Folders as movie files are copied out of the folder. Sometimes files are downloaded with many accompanying files which are not needed. If this is the case then this function can clean up the unused files. [**It is configured here**](https://www.tvrename.com/manual/options#the-folder-deleting-tab).
  * _‘Clean-Up’_ - Files and folders in the download directory that match episodes already in the library. This is useful when something else keeps hold of the lock on the files and they cannot be removed after the move operation, but occasionally deletes ‘PROPER’ or improved files that are improvements to what is already in the library. [**It is setup here**](https://www.tvrename.com/manual/options#the-folder-deleting-tab).
  * Suggest recycling files/folders rather than deleting [**as specified here**](https://www.tvrename.com/manual/options#the-folder-deleting-tab).
* _Multi-episode Merging_
  * Proactive. In the settings (here) TV Rename can be pro-actively setup to create merge rules. If a downloaded or library file matches a multi episode file [(**see here**)](https://www.tvrename.com/manual/options/#the-scan-options-tab) then it will automatically create a merge rule.
  * Reactive. Under the beta option, ‘Duplicate finder’ will scan the library and look for files that look like they are multi-episode files based on a few criteria:
    * The two(or more) episodes have the same air-date
    * The episodes name is similar.
    * One or more of the episodes are missing.
    * The file that is on disk is larger than normal which would indicate that there is more than one episode in the file.
* _Auto-update_
  * On start-up TV Rename will check to see whether it is on the latest version and suggest that it is updated if not.
  * From “Help” in the menu bar you can manually check for an update.
* _Auto Scanning_
  * As files change or on a fixed period (set in [**Options>Settings Search Folders**](https://www.tvrename.com/manual/options#the-search-folders-tab)).
* _Auto Upgrades_
  * As better quality files are identified then they are used to replace lesser quality versions.

[Return to Top](https://www.tvrename.com/manual/features/)

### Exporting <a href="#exporting" id="exporting"></a>

#### Functionality <a href="#functionality-3" id="functionality-3"></a>

TV Rename can be setup to automatically export files which summarise the status of your library.

| **Type**               | **Formats**               | **Description**                                                                                                                                                                                              |
| ---------------------- | ------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| When to Watch          | RSS, XML, iCal            | Details all the upcoming episodes so that you know what episodes are going to air soon. Output whenever information from [The TVDB](http://thetvdb.com) about airdates is updated.                           |
| Missing                | XML, CSV                  | Whenever a full scan is executed TV Rename outputs details of all missing episodes.                                                                                                                          |
| Renamed files          | XML                       | For each scan TV Rename can provide a summary of all renamed files.                                                                                                                                          |
| Copied and Moved files | XML                       | For each scan TV Rename can provide a summary of all moved/copied files.                                                                                                                                     |
| Show List              | TXT, HTML                 | Whenever a show is added or removed from the library TV Rename will update the show list file. The HTML version is a pretty output designed to be printed and viewable by users to help decide what to watch |
| Recent Playlists       | M3U, M3U8, WPL, ASX, XSPF | A playlist file of recently aired shows to be cued up in your favourite media player                                                                                                                         |

#### Further Information <a href="#further-information-5" id="further-information-5"></a>

Further information can be found [**here**](https://www.tvrename.com/manual/options/#the-automatic-export-tab).
