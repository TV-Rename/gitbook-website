---
description: The Quick-Start Guide will help you with the initial setup TV Rename.
---

# Quick Start Guide

To return to this page click `Quickstart Guide` in TV Rename’s **Help**, or browse to [https://www.tvrename.com/manual/quickstart](https://www.tvrename.com/manual/quickstart).

In a nutshell TV Rename will identify, move and rename media files from one folder (or group of folders) to another folder, partially identified by the settings in TV Rename and partially identified from the file name.

Once TV Rename knows about these folders (more on this later) it will process media files and move them to the specified location.

for example: -

The file:

**c:\users\me\downloads\the-outpost-s01e06-hdtv-x264.mkv**

could be “renamed” to:

**m:\TV Series\The Outpost\Season 1\The Outpost - S01E06 - The Book of Names.mkv**

To do this TV Rename uses data acquired from [The TVDB](http://thetvdb.com).

The initial setup can be somewhat daunting as there are many options and settings that control the way TV Rename behaves. Luckily these have sensible defaults and its actually relatively easy to get up and running providing you don’t get distracted by the settings.

{% hint style="info" %}
_The guide assumes you already have the beginnings of a **Media Library** - a folder (or folders) somewhere on your PC or NAS or whatever, with a bunch of tv show files in it (them). TV Rename doesn’t care how these folders are organised, however to us mere humans probably “one folder per show” or “one folder per show with one sub-folder per season” would make sense in terms of being able to (manually) find stuff later if you really need to._
{% endhint %}

## 1 - Add content from your Media Library <a href="#add-content-from-your-media-library" id="add-content-from-your-media-library"></a>

Under normal circumstances you would add a Media Library path when adding a new show to TV Rename, however TV Rename has a trick up its sleeve when adding shows already in the library’s folder infrastructure - **Bulk Add Shows**.

![Tools>Bulk Add Shows](https://www.tvrename.com/assets/images/tools/bulk-add-shows-01.png)

1.  Follow the menu to **Tools>Bulk Add Shows** and whilst on the _**Folders**_ tab of the newly opened window click `Add`. Browse to the root folder of your “Media Library” and click `OK`. The path will be added to the “Monitor Folders” list.

    If you use multiple disks or paths for your library, repeat the above step for each root path.
2. Click the `Check >>` button, the selected path(s) will be scanned and any content with a recognised structure automatically displayed in the _**Scan Results**_ tab.
3.  In the _**Scan Results**_ tab, click `Auto ID All` and TV Rename will attempt to match the found content against [TheTVDB](http://thetvdb.com), and ascertain if the show is part of a “flat” structure with all the episodes in one folder, or a “tree” structure with sub folders for each season and specials.

    Any shows not identified will not have an entry in the **Show** column or the **thetvdb code** column; these can be fixed manually by highlighting the relevant row in the table and clicking `Edit` and using `Search` to interrogate [TheTVDB](http://thetvdb.com).
4. Once the match process has finished, click `Add & Close` and accept the confirmation, all the identified shows will be added to the _**My Shows**_ tab.
5. _**My Shows**_ will now be populated with the TV shows that have been identified, however there is currently no “Season” information. click `Refresh` and all the season information will be downloaded (depending on the size of your media library this may take a little while).
6. Once the download is complete you can browse the series information. Here, by right clicking on a show or season, you can edit the TV Rename settings to override information fetched from [The TVDB](http://thetvdb.com) .
7. You can manually add shows by clicking the `Add` button in the _**My Shows**_ tab. in the _Add/Edit Show_ window that appears enter the show name or code in the” [The TVDB](http://thetvdb.com) code:” box and click `Search` to find it. Hop across to the _**Folders**_ tab and enter the base folder for the show in your media library, and click `OK`.

## 2 - Set your Search Folders <a href="#set-your-search-folders" id="set-your-search-folders"></a>

Whilst not strictly necessary at this point TV Rename needs to know where to look for new files to move to the library when adding new episodes, so lets do it now.

![Options>Preferences>Search Folders](https://www.tvrename.com/assets/images/options/preferences-search-folders-02.png)

In **Options>Preferences**, go to the _**Search Folders**_ tab and `Add` the locations you normally use for new episodes.

For example: I have two entries here, one points to my _Downloads_ folder for stuff I get from the internet. The other points to my _Desktop_ which I use as a target when ripping from my DVD collection.

## 3 - Check the Filename Template

Right, so now TV Rename knows where you media library is and where to look for new files, the only thing it doesn’t know is how you want your files renamed.

Go to the _**Scan**_ tab and select a show that has some season and episode data (for this example I selected the DC show “Arrow”).

Now go to **Options>Filename Template Editor** and you can see how the show will be named.

![Options>Preferences>Search Folders](https://www.tvrename.com/assets/images/options/filename-template-editor-01.png)

The “Sample and Test” pane shows you how the shows episodes will be named using the current naming template.

You can also experiment with other preset templates using the “Presets” drop-down.

If none of these is exactly what you are looking for you can “Roll-your-Own” using the “Tags” drop-down to modify the current template.

[Return to Top](https://www.tvrename.com/manual/quickstart/)

The basic setup is now complete. Now would be a good time to take a look at the other tabs in **Options>Preferences** (if you haven’t already!) to get an idea of how TV Renames behaviour can be customised.

## Ongoing Monitoring <a href="#ongoing-monitoring" id="ongoing-monitoring"></a>

Go to the _**When to watch**_ tab and you will see all known future information (including air dates) for shows you are following.

In the _**Search Folders**_ tab of **Options>Preferences** you can schedule scans, either time based _(“Schedule a scan…)”_ or by gleaning search folder updates from Windows _(“Monitor folders for changes”)_.

**Sit back, relax, and let TV Rename do all the hard work for you!**

_**Whatever changes TV Rename makes to your media file names the season and episode details will remain untouched.**_

_It is highly unlikely that the names of the recordings will get screwed up, but, should it happen, the problem should be easily fixable after changing some settings, or adding new rules. At least, that’s the theory!_\
