# Adding Movies & TV Shows

TV Rename will track many TV Shows and Movies in your library. These can be added in 4 key ways:

* _**Manually**_ – Added manually by entering the name into the ‘Add Show’ screen from the main ‘**TV Shows**’ tab (or equivalent on the **Movies** tab)
* _**Suggestions -**_ TV Rename can make suggestions of other media you want to add to your collection.
* _**Bulk Add**_ – TV Rename can scan through some specified folders (Monitor Folders) via the ‘[Bulk Add](../../menu/tools-menu/bulk-add.md)’ tool. It will display a list of shows that are not already in the library and allow them to be added en-masse.
* _**Automated**_ – TV Rename can be setup to look at files in the download folder (Search Folders) and (if it can’t find an appropriate show in the library) offer the user some suggestions about which series/show to add to the library.

Movies can also be added using the [**Scan Movie Folder**](../../menu/tools-menu/scan-movie-folder.md) option.

### **Manual Addition**

Manual addition is the simplest way of adding shows into the library. You can enter (and search for) the show by name or for more precise addition enter a TVDB Id. All the options about the show can be edited, but they key ones to add are:

* Directory location to store the location of the files for the series
* Time zone for the series (this is not available from TVDB, so must be entered manually)

{% content-ref url="../../main/my-tv-shows.md" %}
[my-tv-shows.md](../../main/my-tv-shows.md)
{% endcontent-ref %}

{% content-ref url="../../main/movies.md" %}
[movies.md](../../main/movies.md)
{% endcontent-ref %}

### **Suggestions**

TV Rename can make suggestions of other media you want to add to your collection:

* **Recommendations** - TV and Movie recommendations from TMDB. (more info [here](../../menu/tools-menu/recommendations.md))
* **Movie Collections** - List all collections your movies are in to allow you to add others from the same collection. (more info [here](../../menu/tasks/movie-collection-summary.md))
* **YTS Movie Recommendations** - (Beta mode only) These 2 tools help discovery of new movies you may be interested in. (more info [here](../../menu/beta-menu.md#yts-movies-and-recommendations))

### **Bulk Addition**

TV Rename can search through your library of existing (organised) files to find shows that are not in the library. This is started from the **Tools** menu. Its options are on the [Scan Settings](../../menu/preferences.md#scan-settings) tab of **Options>Preferences**, in the **Bulk Add TV Shows from Library Folders** group, where it can be set to skip folders with no video files and the Recycle Bin. Specific folders can be skipped by adding them to the **Ignore** tab of the Bulk Add window.

{% content-ref url="../../menu/tools-menu/bulk-add.md" %}
[bulk-add.md](../../menu/tools-menu/bulk-add.md)
{% endcontent-ref %}

### [**Automated** ](automating.md)**Addition**

TV Rename can look at ‘spare’ files in the ‘download’/Search folders;

* If it cannot find a home for them then
* It tries to find the series on TVDB and asks the user for clarification via a streamlined add dialog.
* Once accepted, TVR automatically adds the show.
* If auto folder creation is on, then the folders get created in the library automatically and the appropriate files copied in.

{% hint style="info" %}
This function can be turned on using the **Notify when new media is found** tick box on the [Search Folders](../../menu/preferences.md#the-search-folders-tab) tab of **Options>Preferences**, in the **Auto Add Movies & TV Shows from Search Folders** group. The same group has **Ignore suffixes** (terms that are left out, along with anything after them, when TV Rename works out a show name from a file name) and **Movie Terms** (a file whose name contains one of these terms is taken to be a movie, not a TV show).
{% endhint %}

{% content-ref url="../../menu/preferences.md" %}
[preferences.md](../../menu/preferences.md)
{% endcontent-ref %}
