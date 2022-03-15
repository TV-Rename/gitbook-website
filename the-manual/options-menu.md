# Options Menu

One of TV Rename’s strongest (and most confusing) features is its configurability. For the newcomer especially, it’s very easy to get “lost” in the plethora of options and preferences, and give up.

Luckily the “out-of-the-box” defaults work well, and, should you wish to change any of the options or preferences at some future time all the stuff you can “fiddle” with is described here.

### Offline Operation <a href="#offline-operation" id="offline-operation"></a>

If **Offline Operation** is enabled TV Rename will firstly prompt you to make sure you wish to go offline, and if you click `Yes` it will run on locally cached data from [The TVDB](http://thetvdb.com). This will stop TV Rename attempting to update.

[Return to Top](https://www.tvrename.com/manual/options/)

### Automatic Background Download <a href="#automatic-background-download" id="automatic-background-download"></a>

If **Automatic Background Download** is enabled any action that reads data from the cache will also trigger an update from[The TVDB](http://thetvdb.com), additionally updates will be performed at regular intervals.

### Ignore List <a href="#ignore-list" id="ignore-list"></a>

![The Edit Ignore List window](https://www.tvrename.com/assets/images/options/edit-ignore-list-01.png)When a _**Scan**_ is run any “missing” episodes for shows in your media library are listed.

These may be genuine missing episodes or they may be “Specials”, that don’t fit the season/episode pattern but are still part of the show, for example: -

> My Favourite Show - S00E03 - Recap of Last Season

This may be something you want or it may just be adding to the “noise” in the _**Scan**_ tab.

If it is “noise” you can highlight the row (or multiple rows if that fits better) and right click. A cut-down menu appears, if you select “Ignore Selected” the item is removed from the _**Scan**_ results and appears in the “Ignore List”.

If, at a later date, you decide you wish to add the item, you can remove it from the Ignore list using the _Edit Ignore List_ window, selecting the item in question and clicking `Remove`.

[Return to Top](https://www.tvrename.com/manual/options/)

### Filename Template Editor <a href="#filename-template-editor" id="filename-template-editor"></a>

![The Filename Template Editor tab](https://www.tvrename.com/assets/images/options/filename-template-editor-01.png)This is where the format of the filenames that TV Rename will rename to are defined.

To help illustrate the results the “Sample and Test:” panel contains the processed entries from the show and season selected in the _**My Shows**_ tab.

The “Naming template:” text box displays a tokenised version of the filename which can be edited directly or populated using the “Tags:” drop-down, or overwritten with a record selected from the “Presets:” drop-down. Any changes in the “Naming Template:” are automatically reflected in the “Sample and Test:” panel.

The available tags with their definitions are listed below: -

| {ShowName}       | Name of the Show                                                                                                                          |
| ---------------- | ----------------------------------------------------------------------------------------------------------------------------------------- |
| {Season}         | Number of the season                                                                                                                      |
| {Season:2}       | Number of the season forced to 2 characters with a leading zero                                                                           |
| {Episode}        | Number of the episode (within a season), eg S01E03                                                                                        |
| {Episode2}       | Number of the second episode of a pair (within a season), eg S01E04-E05                                                                   |
|                  | created by the default S{Season:2}E{Episode}\[-E{Episode2}])                                                                              |
| {EpisodeName}    | Name of the Episode                                                                                                                       |
| {Number}         | Overall number of the episode                                                                                                             |
| {Number:2}       | Overall number of the episode forced to 2 characters with a leading zero                                                                  |
| {Number:3}       | Overall number of the episode forced to 3 characters with leading zero(s)                                                                 |
| {SeasonNumber}   | Some season numbers do not start at 1, eg they may go 2012,2013,2014. {SeasonNumber} is the nth season, so would be 1,2,3 in this example |
| {SeasonNumber:2} | As above, but forced to 2 characters with a leading zero                                                                                  |
| {ShortDate}      | Air date in short format, eg 25/12/2017                                                                                                   |
| {LongDate}       | Air date in lomg format, eg 25 December 2017                                                                                              |
| {YMDDate}        | Air date in YMD format, eg 2017/12/25                                                                                                     |
| {AllEpisodes}    | All episodes - E01E02 etc                                                                                                                 |

| _Default:_ | _**{ShowName} - S{Season:2}E{Episode}\[-E{Episode2}] - {EpisodeName}**_ |
| ---------- | ----------------------------------------------------------------------- |
|            | (the second preset).                                                    |

[Return to Top](https://www.tvrename.com/manual/options/)

### Search Engines <a href="#search-engines" id="search-engines"></a>

![The Modify Search Engines window](https://www.tvrename.com/assets/images/options/modify-search-engines-01.png)The _Modify Search Engines_ window controls TV Rename’s outgoing interface with the world (other than TheTVDB). Here, you can configure how and where TV Rename points a web browser searching for files.

Using the `Add` and `Delete` buttons you can create or remove records at will, and the `Tags...` pop up a list of supported tags to remind you whats available. (The tags supported are the same as those listed in the [Filename Template Editor](https://www.tvrename.com/manual/options/#filename-template-editor).)

As an example, here is a URL entry for Google.

> https://www.google.co.uk/search?q={ShowName}+S{Season:2}E{Episode}

The list of URL’s can be used when the _**When to watch**_ tab is open, the last used entry becomes the default, and appears in a text box to the right of the `Refresh` button. It can be changed by clicking the `▼` button and selecting another entry.

With a little ingenuity you can get really creative with these entries and pass your search to its specific target through a web proxy.

[Return to Top](https://www.tvrename.com/manual/options/)

### Filename Processors <a href="#filename-processors" id="filename-processors"></a>

![he Filename Processors window](https://www.tvrename.com/assets/images/options/filename-processors-01.png)In much the same way that the _**Filename Template Editor**_ is used to process the names of files being moved to the media library so _**Filename Processors**_ is used to inform TV Rename what filenames to look out for when searching for a missing files

To really understand the contents of the Regex column above, you need a working knowledge of [Regular Expressions](https://regexone.com).

Once you have figured out whats going on you can see that all the regular expressions capture the season and episode number of a show from the filename. Each one can work on just the filename: -

> ShowName S01E07.avi

or on the whole path: -

> C:/files/ShowName/S01E07.avi

The expressions are evaluated in order (top down).

Each expression can be toggled on and off, as can the ability to process a full path.

Each expression has a Notes field which can be used to remind the user why the expression was added.

Additionally, a folder can be specified to test the results of the Regular Expression.

If a match is found during the test the matching expression is indicated.

In all likelihood you will find it unnecessary to make changes here, only if a new, totally unrecognisable file name structure appeared would it be necessary, and then there would probably be discussion about it in the forum.
