# Quick Rename TV Files

**Quick Rename TV Files** renames TV episode files in the folder they are already in, using your [filename template](../options-menu/filename-template-editor.md). It is useful for a few files outside your library, for example on a USB stick, that you want named properly without moving them anywhere.

1. Choose **Tools > Quick Rename TV Files...**. The **Format** box shows the template that will be used (change it with the Filename Template Editor).
2. Pick the **Show**. Leave it on `<Auto>` to let TV Rename work out the show from each file's name and path, or choose a show from your library to use for every file you drop.
3. Drag files, or whole folders, onto **Drop Files Here**. Folders are searched including all their subfolders.
4. Go to the **Scan** tab in the main window. Each file that was matched is listed under **Move** (it stays in the same folder; only its name changes). Check the new names, then click `Do Checked`.

The Quick Rename window can stay open while you work, and anything else you drop is added to the same list.

Things to know:

* Opening Quick Rename clears any results already on the **Scan** tab.
* Only video files are considered (the file types set in [Preferences > Files and Folders](../preferences.md#the-files-and-folders-tab)). A file that can't be matched to a show, season and episode is skipped, and the reason is written to the log. A file that already has the right name is left alone.
* If the show isn't in your library yet and **Auto-Add as part of Quick Rename** is ticked (Preferences > General, on by default), TV Rename tries to identify the show and add it, asking you to confirm.
* If **Copy files, don't move** is ticked in [Preferences > Search Folders](../preferences.md#the-search-folders-tab), a renamed copy is made next to the original instead, and it is listed under **Copy**.
* Your other settings still apply, so TV Rename may also offer to create NFO files or thumbnails for the renamed episodes, and to bring along files with the same name (such as subtitles), if those options are on.
