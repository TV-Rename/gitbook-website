# Force Refresh All Images

**Force Refresh All Images** downloads fresh artwork for every TV show and movie in your library and replaces the image files already on disk. Use it if your artwork is out of date or broken, or after you change which images TV Rename should save.

Which images it fetches depends on what is switched on in [Preferences > Media Centres](../preferences.md#the-media-centers-tab), for example `folder.jpg`, `fanart.jpg`, `series.jpg`, episode thumbnails and the Kodi images. If none are ticked there is nothing for it to do.

1. Choose **Tools > Force Refresh All Images**. Any results already on the **Scan** tab are cleared, and a progress window works through your shows and then your movies.
2. When it finishes, the **Scan** tab opens with every image to download listed under **Download**.
3. Nothing has been downloaded yet. Untick anything you want to leave as it is, then click `Do Checked`.

Things to know:

* Only shows and seasons whose folders exist on disk are included. Ignored seasons are skipped, and so are Specials if they are set to be ignored for all shows.
* For a movie, images are refreshed for each movie file in its folder.
* If TV Rename is busy downloading updates from the data sources you will see "Can't refresh until background download is complete". Wait until the status bar shows the background download is idle and try again.

{% hint style="info" %}
This refreshes image files only. To refresh the show and movie information itself, see [Force Refresh All](force-refresh-all.md).
{% endhint %}
