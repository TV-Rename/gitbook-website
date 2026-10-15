# Automatic Background Download

When **Options > Automatic Background Download** is ticked, TV Rename keeps its show and movie information up to date by itself. It checks TheTVDB, TMDB and TVmaze for changes to the shows and movies in your library and downloads anything that has changed:

* about 10 seconds after TV Rename starts, and then
* every few hours, as set by **Update cache every ... hours** on the [Data Sources](../preferences.md#data-sources) tab of Preferences. The default is every hour.

While it runs, the right-hand side of the [status bar](../../main/other.md#the-status-bar) shows what is being downloaded. When it finishes, TV Rename saves the information it downloaded and updates the **Schedule** tab.

If TV Rename is already busy downloading when an update is due, it waits and tries again later.

Untick it to stop the regular updates. You can still update whenever you like with [Tools > Background Download Now](../tools-menu/background-download-now.md) (Ctrl+B), and TV Rename still downloads the information it needs when you scan or add a show.

{% hint style="info" %}
To work only with the information TV Rename already has, see [Offline Operation](offline-operation.md).
{% endhint %}
