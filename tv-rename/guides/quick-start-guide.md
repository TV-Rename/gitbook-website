---
description: The Quick-Start Guide will help you with the initial setup TV Rename.
---

# Quick Start Guide

To return to this page click `Quickstart Guide` in TV Rename’s **Help**, or browse to [https://www.tvrename.com/guides/quick-start-guide](https://www.tvrename.com/guides/quick-start-guide).

In a nutshell, TV Rename will identify, move and rename media files from one folder (or group of folders) to another folder, partially identified by the settings in TV Rename and partially identified from the file name.

Once TV Rename knows about these folders (more on this later) it will process media files and move them to the specified location.

for example: -

> The file:
>
> **c:\users\me\downloads\the-outpost-s01e06-hdtv-x264.mkv**
>
> could be “renamed” to:
>
> **m:\TV Series\The Outpost\Season 1\The Outpost - S01E06 - The Book of Names.mkv**
>
> To do this TV Rename uses data acquired from [TMDB](https://www.themoviedb.org/), [The TVDB](http://thetvdb.com/) and [TVmaze](https://www.tvmaze.com/) (see [Data Sources](../help-and-support/data-sources.md)).

The initial setup can be somewhat daunting as there are many options and settings that control the way TV Rename behaves. Luckily these have sensible defaults and its actually relatively easy to get up and running providing you don’t get distracted by the settings.

{% hint style="info" %}
_The guide assumes you already have the beginnings of a **Media Library** - a folder (or folders) somewhere on your PC or NAS or whatever, with a bunch of movie or tv show files in it (them). TV Rename doesn’t care how these folders are organised, however to us mere humans probably “one folder per show” or “one folder per show with one sub-folder per season” would make sense in terms of being able to (manually) find stuff later if you really need to._
{% endhint %}

## 1 - Add content from your Media Library <a href="#add-content-from-your-media-library" id="add-content-from-your-media-library"></a>

### Bulk Add (best if you have a folder of sorted media files)

Under normal circumstances you would add a Media Library path when adding a new show to TV Rename, however TV Rename has a trick up its sleeve when adding shows already in the library’s folder infrastructure - **Bulk Add TV Shows**.

<figure><img src="../.gitbook/assets/image (50).png" alt=""><figcaption></figcaption></figure>

1.  Follow the menu to **Tools>Bulk Add TV Shows...** and whilst on the _**Folders**_ tab of the newly opened window click `Add`. Browse to the root folder of your “Media Library” and click `OK`. The path will be added to the “Monitor Folders” list.

    If you use multiple disks or paths for your library, repeat the above step for each root path.
2. Click the `Check >>` button, the selected path(s) will be scanned and any content with a recognised structure automatically displayed in the _**Scan Results**_ tab.
3.  In the _**Scan Results**_ tab, click `Auto ID All` and TV Rename will attempt to match the found content against your default data source (TMDB, unless you have changed **Default TV Show Source** on the [Data Sources](../menu/preferences.md#data-sources) tab of **Options>Preferences**). The **Folder Structure** column shows whether each show is “Flat”, with all the episodes in one folder, or “Folder per season”, with sub folders for each season and specials.

    Any shows not identified will not have an entry in the **Show** column or the **Source Code** column; these can be fixed manually by highlighting the relevant row in the table and clicking `Edit` and using `Search` to look the show up.
4. Once the match process has finished, click `Add & Close` and accept the confirmation, all the identified shows will be added to the _**TV Shows**_ tab.
5. TV Rename then downloads the information for the new shows, including their seasons and episodes (depending on the size of your media library this may take a little while), and the _**TV Shows**_ tab fills in.
6. Once the download is complete you can browse the series information. Here, by right clicking on a show or season, you can edit the TV Rename settings to override information fetched from the data source.

### Manually

1. You can manually add shows by clicking the `Add` button in the _**TV Shows**_ tab. In the [_Add/Edit Show_](../main/my-tv-shows.md#addedit-show) window that appears enter the show name, or its code at the data source, in the code box (labelled for the data source, for example “TMDB code:”) and click `Search` to find it. Hop across to the _**Folders**_ tab and enter the base folder for the show in your media library, and click `OK`.

## 2 - Set your Search Folders <a href="#set-your-search-folders" id="set-your-search-folders"></a>

Whilst not strictly necessary at this point TV Rename needs to know where to look for new files to move to the library when adding new episodes, so lets do it now.

<figure><img src="../.gitbook/assets/image (61).png" alt=""><figcaption></figcaption></figure>

In [**Options>Preferences**](../menu/preferences.md#the-search-folders-tab), go to the _**Search Folders**_ tab and `Add` the locations you normally use for new episodes.

For example: I have two entries here, one points to my _Downloads_ folder for stuff I get from the internet. The other points to my _Desktop_ which I use as a target when ripping from my DVD collection.

## 3 - Check the TV Filename Template

Right, so now TV Rename knows where you media library is and where to look for new files, the only thing it doesn’t know is how you want your files renamed.

Go to the _**TV Shows**_ tab and select a show that has some season and episode data (for this example I selected the DC show “Arrow”).

Now go to **Options>Filename Template Editor** and you can see how the show will be named.

<figure><img src="../.gitbook/assets/image (59).png" alt=""><figcaption></figcaption></figure>

The “Sample and Test” pane shows you how the shows episodes will be named using the current naming template.

You can also experiment with other preset templates using the “Presets” drop-down.

If none of these is exactly what you are looking for you can “Roll-your-Own” using the “Tags” drop-down to modify the current template.

{% hint style="info" %}
The basic setup is now complete. Now would be a good time to take a look at the other tabs in **Options>Preferences** (if you haven’t already!) to get an idea of how TV Renames behaviour can be customised.
{% endhint %}

{% content-ref url="../menu/options-menu/filename-template-editor.md" %}
[filename-template-editor.md](../menu/options-menu/filename-template-editor.md)
{% endcontent-ref %}

## 4 - Run a Scan <a href="#ongoing-monitoring" id="ongoing-monitoring"></a>

Now you’re ready to run your first scan.

Go to the _**Scan**_ tab, and click `Full Scan` (if the window is narrow, click the arrow next to `Scan` and choose `Full`). TV Rename will download any needed show information from its data sources, and compare it with the contents of the media library.

<figure><img src="../.gitbook/assets/image (52).png" alt=""><figcaption></figcaption></figure>

When the scan is complete, TV Rename will display its suggested changes in the main pane. Any ticked item will be actioned, so un-tick things you’re not sure about, or use the `Check` drop-down on the toolbar to tick or un-tick a whole type of action at once.

For a more “granular” approach you can right-click on selected items to see actions for that specific item.

Click `Do Checked` and TV Rename will process the ticked actions, moving and renaming files as necessary.

{% content-ref url="../main/scan.md" %}
[scan.md](../main/scan.md)
{% endcontent-ref %}

## 5 - Ongoing Monitoring <a href="#ongoing-monitoring" id="ongoing-monitoring"></a>

Go to the _**Schedule**_ tab and you will see all known future information (including air dates) for shows you are following.

TV Rename can also scan for you. On the [_**Scan Settings**_](../menu/preferences.md#scan-settings) tab of **Options>Preferences** you can schedule a time based scan _(“Scheduled scan every … hours”)_, and on the [_**Search Folders**_](../menu/preferences.md#the-search-folders-tab) tab you can have TV Rename scan whenever the contents of your search folders change _(“Monitor Search Folders (run a scan when files change)”)_.

**Sit back, relax, and let TV Rename do all the hard work for you!**

{% hint style="info" %}
_**Whatever changes TV Rename makes to your media file names the season and episode details will remain untouched.**_
{% endhint %}

_It is highly unlikely that the names of the recordings will get screwed up, but, should it happen, the problem should be easily fixable after changing some settings, or adding new rules. At least, that’s the theory!_<br>
