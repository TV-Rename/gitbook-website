# Find Duplicate Movies

![](<../../.gitbook/assets/image (7).png>)

**Find Duplicate Movies** checks every movie in your library and lists the ones that have more than one video file in their folder. It starts as soon as the window opens, with a progress bar while it works.

| Column | What it means |
| --- | --- |
| Movie | The movie in your library. |
| Filenames | The video files found for it. |
| MultiPart Movie | Ticked when there are exactly two files whose names end in a part number, such as `CD1`/`CD2`, `Part1`/`Part2` or `Disc1`/`Disc2` (also `pt`, `dvd` and `disk`). These are normally one movie split in two, not a duplicate. |
| Sample? | One of the files looks like a sample: "sample" is in its name and it is smaller than the sample size limit set in Preferences. |
| Deleted? | One of the files is a tiny leftover stub, such as a macOS `._` file. |
| # files | How many files were found. |

Right-click a row to:

* **Force Refresh**: download this movie's information again, then re-check it.
* **Update**: re-check this movie's folder, for example after you have removed a file yourself.
* **Edit Movie**: open the movie's settings.
* **Choose Best**: keep the best file and delete the others (read the warning below first).
* **Visit** a file: open File Explorer with that file selected.

**How Choose Best decides.** It compares the files' running time and picture width (resolution). A file wins if it is longer or wider by more than the margin set in [Preferences > Search Folders](../preferences.md#the-search-folders-tab) (_Consider a file better if it is X% higher resolution/longer_, 10% by default). If that doesn't separate them, a file whose name contains one of the _Priority override terms_ (`PROPER;REPACK;RERIP` by default) wins. If it still can't tell, or can't read the video details, it asks you which file to keep, or whether to keep both. If the files are identical it keeps one and deletes the other without asking.

{% hint style="danger" %}
**Choose Best deletes the losing file immediately and permanently.** It does not go to the Scan tab for you to confirm, and it does not go to the Recycle Bin, whatever your Folder Deleting settings say. If that leaves the folder with no video files, the folder is then tidied up using your Folder Deleting settings.

**Do not use Choose Best on a MultiPart Movie row.** The two parts are compared like any other pair, so if one part is more than 10% longer than the other, the shorter part is deleted without asking.
{% endhint %}

To re-check the whole library, close the window and open it again.
