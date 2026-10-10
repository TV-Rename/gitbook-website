# Force Refresh Kodi TV Show NFO Files

This rewrites the Kodi `.nfo` information files for your whole library from TV Rename's current data, even where TV Rename thinks they are already up to date. Use it if Kodi is showing old or wrong details, or after you have changed a show's details or its data source.

It covers:

* `tvshow.nfo` in each TV show's folder, if **NFO files for shows** is ticked in [Preferences > Media Centres](../preferences.md#the-media-centers-tab) (Kodi section). This is **off by default**.
* The `.nfo` for each movie file, if **NFO files for movies** is ticked (on by default). Despite the menu name, movies are included.

Episode `.nfo` files are not part of this tool.

A progress window works through your shows and movies, then the **Scan** tab opens with the files to be written listed under **Media Center Metadata**. Click `Do Checked` to write them.

Things to know:

* Shows with no base folder, or none of whose folders exist on disk, are skipped, as are movies with no folder on disk.
* You don't normally need this. During every scan TV Rename already rewrites a show, episode or movie `.nfo` when the information at the data source has changed since the file was written, so occasional NFO actions in your scan results are normal.
