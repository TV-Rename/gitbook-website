# Scan

TV Rename can scan your media library looking for missing or outdated files and will try to repair any issues it finds automatically.

There are three types of scan available : -

<table><thead><tr><th width="125"></th><th></th></tr></thead><tbody><tr><td><strong>Full</strong></td><td>A full scan of all shows and seasons.</td></tr><tr><td><strong>Recent</strong></td><td>A Scan of all the shows that have aired recently.</td></tr><tr><td><strong>Quick</strong></td><td>Scan the shows that have aired recently and have a missing episode in the library. Also check the locations specified in <em>Options>Preferences>Search Folders</em> for any matching media files.</td></tr></tbody></table>

As with other tabs, “recent” is taken as being the number of days counted as recent indicated in the **Options>Preferences** [_**General**_](../menu/preferences.md#the-general-tab) tab.

### Scan Progress

While a scan runs, the **Scan Progress** window shows how far it has got. The scan works through the stages below in order, each with its own progress bar. Stages that your settings don't use are greyed out and skipped.

| Stage                    | What it does                                                                                                      | When it runs                                                                                                                                                                                                                                                                                                               |
| ------------------------ | ----------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Scan Library for New** | Looks in your library folders for shows and movies that aren't in TV Rename yet.                                  | When **Do Bulk-Add as part of scan** is ticked on the [Scan Settings](../menu/preferences.md#scan-settings) tab.                                                                                                                                                                                                           |
| **Media Library Check**  | Checks the files already in your library, for files to rename and episodes or movies that are missing.            | When **Rename Check** or **Missing Check** is ticked on the Scan Settings tab.                                                                                                                                                                                                                                             |
| **Download Area Check**  | Checks your search folders for files that can be tidied up or that are better versions of files you already have. | When one of the **Clean up already copied...** options is ticked on the [Folder Deleting](../menu/preferences.md#the-folder-deleting-tab) tab, or one of the **Update ... when higher-quality ones found in Search Folders** options is ticked on the [Search Folders](../menu/preferences.md#the-search-folders-tab) tab. |
| **Search Locally**       | Looks for missing episodes and movies on your computer.                                                           | When **Missing Check** is ticked and **Look in "Search Folders" for missing files** is ticked on the Search Folders tab. It also looks for misplaced files inside your library when **Move Files within Library to Keep it Tidy**, **Rename Check** and **Missing Check** are all ticked on the Scan Settings tab.         |
| **Search Downloading**   | Checks whether missing episodes and movies are already downloading.                                               | When **Missing Check** is ticked and **Check qBitTorrent queue**, **Check µTorrent queue** or **Check SABnzbd queue** is ticked on the [Torrents / NZB](../menu/preferences.md#torrents-nzb) tab.                                                                                                                          |
| **Search Web**           | Searches the web for downloads of missing episodes and movies.                                                    | When **Missing Check** is ticked and **Search RSS for missing files** or **Search JSON for missing files** is ticked on the [RSS / JSON Search](../menu/preferences.md#rss-json-search) tab, or **Search Jackett for missing files** is ticked on the [Jackett Search](../menu/preferences.md#jackett-search) tab.         |

The lines under the progress bars show what is being checked at that moment. The window closes by itself when the scan finishes. Click `Cancel` to stop the scan.

### Auto create folders

When **Missing Check** is ticked, the scan checks that every season of the shows being scanned has a folder in your library. If a season folder is missing, TV Rename asks you what to do in the **Missing Folder** window.

The window shows:

* **Show:** the show's name.
* **Season:** the season, and the highest season number the show has, for example `3 of 5`.
* **Folder:** the folder TV Rename expected to find.

| Button          | What it does                                                                                                                                                                         |
| --------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `Create`        | Creates the folder and carries on.                                                                                                                                                   |
| `Retry`         | Checks for the folder again. Use this if you have just created or reconnected it yourself.                                                                                           |
| `Browse...`     | Lets you pick a different folder for the season. You can also drag and drop a folder onto the window. If the folder you pick exists, TV Rename remembers it as that season's folder. |
| `Ignore Once`   | Skips the folder for this scan only. You will be asked again next time.                                                                                                              |
| `Ignore Always` | Adds the season to the show's ignored seasons, so TV Rename stops checking it.                                                                                                       |
| `Cancel`        | Stops the scan.                                                                                                                                                                      |

If TV Rename doesn't know which folder to use for the season, the **Folder:** line reads "Click Browse..., or Drag+Drop a folder onto this window." and `Create` and `Retry` are greyed out.

You won't be asked about seasons you have told TV Rename to ignore, or about a season where every episode would be skipped anyway, for example because they are all on the [Ignore List](../menu/options-menu/ignore-list.md) or have been seen before with **Ignore Episodes Previously Seen** ticked.

When TV Rename is started hidden from the [command line](../technical/command-line.md), it skips missing folders without asking.

{% hint style="info" %}
To have TV Rename create missing folders without asking, tick **Automatically create missing folders** on the [Scan Settings](../menu/preferences.md#scan-settings) tab. You will still be asked if a folder can't be created.
{% endhint %}

### Auto-Add (New Show Detected)

If **Notify when new media is found** is ticked on the [Search Folders](../menu/preferences.md#the-search-folders-tab) tab, the scan looks at the video files in your search folders for shows and movies that aren't in TV Rename yet. For each one it finds, it opens the **New Show Detected...** window so you can add it. See [Auto Add Shows](my-tv-shows.md#auto-add-shows) for how to use that window.

Auto-Add only runs on scans you start yourself, not on scans TV Rename runs on its own.

Two more options on the Search Folders tab let TV Rename add a match without asking:

* **Auto Add when only one tv show found** adds the show straight away when only one matching show is found. This also needs **Use Automatic Season Folders** and **Use Default Location** ticked on the [TV Show Defaults](../menu/preferences.md#tv-show-defaults) tab.
* **Auto Add when only one movie found** does the same for movies. This also needs **Use Default Location** ticked, with a location chosen, on the [Movies Defaults](../menu/preferences.md#movies-defaults) tab.

If you haven't set up any library folders, TV Rename shows a **Can't Auto Add Media** message instead. Add a library folder, or turn the option off.

### Upgrade File Quality

<figure><img src="https://3508557057-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2Fx0gPeIfHpbgTioNust1M%2Fuploads%2Foi5rYWaJuviNnzOlua63%2Fimage.png?alt=media&#x26;token=4be37fbf-6324-4dab-ba81-a66b342c6a58" alt=""><figcaption></figcaption></figure>

If the **Update episodes when higher-quality ones found in Search Folders** box (or **Update movies when higher-quality ones found in Search Folders** for movies) is ticked in **Options>Preferences** [_**Search Folders**_](../menu/preferences.md#the-search-folders-tab) and there are two versions of an episode file in the library and/or download location you will be prompted to choose which file to keep when the scan completes as illustrated…

### Choose Download

A web search can find more than one download for the same missing episode or movie. What TV Rename does then is set on the [Jackett Search](../menu/preferences.md#jackett-search) tab of **Options>Preferences**:

* **Supervised Duplicate Action:** is used for scans you start yourself.
* **Unattended Duplicate Action:** is used for scans TV Rename runs on its own, such as a scan on startup, a scheduled scan, a scan started by a change in a monitored folder, or a scan run from the command line.

| Option                  | What happens                                                        |
| ----------------------- | ------------------------------------------------------------------- |
| **Ask User**            | TV Rename opens the **Choose Download** window so you can pick one. |
| **Choose Largest File** | The largest download is used.                                       |
| **Choose Most Popular** | The download with the most seeders is used.                         |
| **Download All**        | Every download found is kept.                                       |
| **Ignore**              | None of them is used, and the episode or movie stays missing.       |
| **Use First**           | The first download found is used.                                   |

The **Choose Download** window shows the episode or movie after **Selected Episode:**, and lists the downloads found for it with their **Name**, **Size**, **Seeders** and **Source**, with the most seeders first.

| Button       | What it does                                                                                              |
| ------------ | --------------------------------------------------------------------------------------------------------- |
| `OK`         | Uses the selected download. You can also double-click a row.                                              |
| `See All`    | Lists every download that was found, including any that were left out of the first list.                  |
| `Cancel`     | Uses none of them. The episode or movie stays missing.                                                    |
| `Cancel All` | Uses none of them, and does the same for any others still to be asked about in this scan, without asking. |

### Scan Results

_**Scan**_ indicates where there are gaps in your library. The result of a typical scan is shown below.

<figure><img src="https://3508557057-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2Fx0gPeIfHpbgTioNust1M%2Fuploads%2F5GEdfbeldYyoUC7Cv7Jz%2Fimage.png?alt=media&#x26;token=76ec19e8-8fc3-4f13-8462-dfe2b5e41e05" alt=""><figcaption></figcaption></figure>

The scan indicates that there a number of missing episodes, a file in the media library that needs to be renamed, a file that has been downloaded and is waiting to be moved to the media library and be renamed in the process and a duplicate file that can be removed.

Looking at the missing episodes first; even here TV Rename is “trying to help”. Note that each entry has a magnifying glass icon to the left of the row. Single clicking one of these rows and then clicking the `Web Search` button (in this case “Zooqle”) will launch a search for the indicated file (configured in [**Options>Search Engines**](../menu/options-menu/search-engines.md)). Double clicking one of these rows will launch the same web search. You an also select multiple rows and then click the `Web Search` button to launch a browser with multiple tabs, one for each highlighted row.

If you’re having trouble finding what you’re searching for you can change the search engine to another in the [**Options>Search Engines**](../menu/options-menu/search-engines.md) list by clicking the `▼` button next to “Web Search” and selecting a different entry.

In addition to the files to be searched for, the _**Scan**_ tab is also showing that there is one file to be renamed and one file to be copied or moved (see the **Options>Preferences** [_**Scan Settings**_](../menu/preferences.md#scan-settings) tab). Note both items have a tick in the box icon to the left of each row.

### Scan Results Options

There are also a number of useful options available in the right-click menu here.

Selecting files in the main scan panel and clicking `Ignore Selected` will remove them from the system (permanently unless they are removed from the ignore list - see [**Options>Ignore List**](../menu/options-menu/ignore-list.md)).

Selecting files in the main scan panel and clicking `Revert to Missing` will mark (and list) them as missing. (If they are within the date range of “Aired in the last…” in the _**Schedule**_ tab they will also be shown as missing there.

Selecting files in the main scan panel and clicking `Remove Selected` will temporarily remove them from the scan tab. They will re-appear when the scan is re-run.

In addition you can toggle individual items on or off by clicking directly on their tick boxes.

### Execute Actions

When the `Do Checked` button is clicked everything ticked will be processed.

Note that there are some tick boxes to the right of the buttons. These give you course control over the ticked items, it this case we can toggle everything to be moved and/or everything to be renamed on and off.

Once you are happy with everything selected click on `Do Checked` and the Copy/Move/Rename process will start.

<figure><img src="https://3508557057-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2Fx0gPeIfHpbgTioNust1M%2Fuploads%2FoZnCFnP9JxPk3zjyXRxm%2Fimage.png?alt=media&#x26;token=c1caf9c3-0e95-46cd-a3e0-64732ef46ad9" alt=""><figcaption></figcaption></figure>

While files are being copied and/or moved, this dialog is shown. Click `Pause` to temporarily pause the copy/move operation. Click it again to resume. Clicking `Cancel` will stop the operation immediately. The disk space shown is for the drive that the current file is being copied/moved to.
