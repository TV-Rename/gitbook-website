# Beta Menu

The **Beta** menu appears between **View** and **Help** when **Mode** is set to **Beta** in [Preferences > General](preferences.md#the-general-tab). Its tools are previews of features still being worked on.

## Functions that report into the logs

These tools write their results to TV Rename's log. Each one opens the **TV Rename Log Viewer** window (the same window as **Help > Log**) so you can watch the results arrive. The results are also kept in the log file, see [Logs & Configuration](../technical/logs-and-configuration.md).

### Timezone Inconsistency (Log)

Produces a table in the log file that identifies shows with an incorrect timezone. An incorrect timezone prevents air times from converting to your local timezone. The table summarises networks whose shows use multiple timezones. Networks normally use one consistent timezone for episode airings.

### Episode File Quality Summary (Log)

Lists every episode file in your library with its video width and height in pixels and its length in seconds, followed by the show name and the file name. Use it to spot episodes that are lower quality, or much shorter or longer, than the rest. For example:

```
1920         1080         1751          Mortimer & Whitehouse - Gone Fishing     Mortimer & Whitehouse - Gone Fishing.S08E01.mkv
```

The list starts with `File Quality FINDER - Start` and ends with `File Quality FINDER - End`. A file TV Rename can't read the video details from, such as a `.strm` file, is listed with `-1` in each of the first three columns, and a warning about it is also added to the log.

Every episode file is opened to read its details, so this can take a while for a large library.

### TVDB Accuracy Check (Log) and TMDB Accuracy Check (Log)

These compare the information TV Rename has stored for your shows and movies with what is currently on the data source's website, and download again anything that is out of date.

* **TVDB Accuracy Check (Log)** checks the shows and movies that use TheTVDB as their data source.
* **TMDB Accuracy Check (Log)** checks the shows and movies that use TMDB as their data source.

The differences found are written to the log, and the out-of-date shows and movies are then refreshed. Every show and movie is checked against the website, so this can take a while for a large library.

### TVDB Update Checker (Log)

Shows what TheTVDB has recorded as changed for one show since a time you choose. It is useful when a change you expect on TheTVDB, such as a new episode, has not appeared in TV Rename yet.

1. Choose **Beta > TVDB Update Checker (Log)**. The **TVDB Updates Checker** window opens.
2. Pick the **TV Show**. Only shows that use TheTVDB as their data source are listed.
3. Set the **Time**. It starts at the last update time TV Rename has stored for that show.
4. Click `OK`. The Log Viewer opens and lists each change TheTVDB recorded for the show, its seasons and its episodes since that time. `Cancel` closes the window without checking.

## YTS Movies and Recommendations

2 tools that allow you to see ideas of new movies that you might be interested in:

* **YTS Movie Recommendations** - Uses your current library to propose other movies that are similar that you may like
* **YTS Movie Preview** - Looks at all available movies
