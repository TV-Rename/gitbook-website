# Move Movies From...

**Move Movies From...** takes a folder of movie files that is **not** one of your library folders, such as a download folder, an external drive or a folder someone has given you, and files the movies into your movie library, renamed to your movie naming format.

1. Choose **Tools > Move Movies From...** and pick the folder.
2. TV Rename checks every video file in that folder and all its subfolders. Samples (if you have set TV Rename to ignore them) and tiny leftover stub files are skipped.
3. For each movie file:
   * If it looks like a movie already in your library, you are asked which movie it is. Pick the movie, choose to add it as a new movie, or Cancel to skip that file.
   * If it doesn't look like anything in your library, TV Rename tries to identify the movie and add it, asking you to confirm.
4. When it has finished, the **Scan** tab opens with the proposed actions. Nothing has been moved yet: check the list, then click `Do Checked`.

What it proposes for each file:

* **The movie's library folder doesn't have it yet:** the file is moved into the movie's folder and renamed. If **Copy files, don't move** is ticked in [Preferences > Search Folders](../preferences.md#the-search-folders-tab), it is copied instead and the original stays where it is.
* **The library already has a copy:** the two files are compared the same way as [Find Duplicate Movies](find-duplicate-movies.md) does (running time, resolution and the priority override terms). If the new file is better it replaces the library copy. If TV Rename can't tell, it asks you.
* **The library copy is as good or better:** the new file is listed under **Remove**, so it can be cleared out of the source folder (deleted or recycled according to your Folder Deleting settings). Untick it if you want to keep it.

Files with the same name (such as subtitles) and subtitle folders come along too if those options are on, and NFO files and artwork are created as set in Preferences > Media Centres.

{% hint style="warning" %}
This is not a replacement for a normal scan, and it can't be pointed at one of your library folders (TV Rename stops and tells you so). To bring movies that are already in your library folders into TV Rename, use [Bulk Add](bulk-add.md).
{% endhint %}
