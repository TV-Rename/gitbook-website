# Settings Check

When you add a show or movie, TV Rename gives it the defaults set in [Preferences](../preferences.md) (the **TV Show Defaults** and **Movies Defaults** tabs). Over time you change some of them for individual shows and movies: a custom name here, DVD order there, a movie kept in its own folder. **Settings Check** finds every show and movie whose settings no longer match your defaults and lists them in one place, so you can review them and put back any you no longer want.

## When to use it

* **After changing your defaults.** New defaults only apply to shows and movies you add afterwards. Settings Check shows which existing ones still use the old settings.
* **Tidying up.** Find the one-off changes you made years ago and have forgotten about.
* **Before reorganising your library folders.** See which shows and movies have their own folder arrangements, so nothing surprises you.

## A few terms

| Term              | Meaning                                                                                                                                |
| ----------------- | -------------------------------------------------------------------------------------------------------------------------------------- |
| Defaults          | The settings in **Preferences > TV Show Defaults** and **Preferences > Movies Defaults**. Every new show or movie starts with these.   |
| Data source       | Where TV Rename gets a show's or movie's information: [TheTVDB, TMDB or TV Maze](../../help-and-support/data-sources.md).              |
| Library folder    | A top-level folder that holds your shows or movies, set in [Preferences > Library Folders](../preferences.md#the-library-folders-tab). |
| Base folder       | A show's or movie's own folder inside a library folder. A show's season folders go inside it.                                          |
| Automatic folders | TV Rename works out the folder names itself, from your folder naming settings.                                                         |
| Manual folders    | You have pointed TV Rename at specific folders yourself, on the show's or movie's **Folders** tab.                                     |

## Running the check

Choose **Options > Settings Check**. A window titled **Settings Review** opens and the check starts straight away, with a progress bar stepping through each show and movie in your library. Automatic scans are paused while the window is open.

When it finishes, the list shows only the shows and movies that differ from your defaults. They are grouped under the name of each check, with a count, for example **\[TV] Use Custom TV Show Name \[11 items]**. Click the arrow at the right-hand end of a group's heading to collapse or expand it. Click **Refresh** to check again, for example after you have edited a show, and **Close** when you are done.

| Column       | What it shows                                                                       |
| ------------ | ----------------------------------------------------------------------------------- |
| Show / Movie | The show or movie.                                                                  |
| Check        | Which setting differs. TV checks start with `[TV]` and movie checks with `[Movie]`. |
| Type         | `tv` or `movie`.                                                                    |
| Explain      | Your default and this show's or movie's value, side by side.                        |
| Error Text   | Why a fix didn't work, if it didn't.                                                |

{% hint style="info" %}
A setting that differs from your defaults is not necessarily wrong. A show that only matches correctly in DVD order, or a custom name chosen to line up with another app, is usually there on purpose. Only fix the items you did not mean to set.
{% endhint %}

## What it looks for

The checks are grouped below by what they affect. The **Check** column shows the name exactly as it appears in the window.

### What gets scanned, and how files are matched

These are the options on the **Advanced** tab of **Edit TV Show** or **Edit Movie**. Each is listed when the show's or movie's setting is different from your default.

| Setting in Edit TV Show / Edit Movie                        | Check                            |
| ----------------------------------------------------------- | -------------------------------- |
| Do renaming                                                 | Rename Check                     |
| Do missing check                                            | Do Missing Check                 |
| Look for airdate in filenames                               | Do Airdate matching Check        |
| Look for episode title in filenames                         | Do EpisodeName Matching Check    |
| Use sequential number matching                              | Do Sequential Matching Check     |
| Include future episodes                                     | Do Future Episodes Check         |
| Include no airdate                                          | No Airdate Check                 |
| Show next airdate in 'Schedule'                             | Show Next AirDate Check          |
| Specials count as episodes                                  | Count Specials As Episodes Check |
| Use DVD Order                                               | Use DVD Order Check              |
| Use Alternate Order                                         | Use Alternate Order Check        |
| Include check when movie has a future release date (movies) | Do Future Movies Check           |
| Include check when movie has no release date (movies)       | No Airdate Movie Check           |

**Fix Issue** sets the option back to your default.

### Names, language and data source

| Check                                    | Listed when                                                                                          | Fix Issue does this                                                                                            |
| ---------------------------------------- | ---------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------- |
| Use Custom TV Show Name, Use Custom Name | The show or movie uses its own name (on the **Basics** tab) instead of the one from its data source  | Turns the custom name off. If renaming is on, the next scan renames its files to match the data source's name  |
| Use Custom Language, Use Custom Region   | The show or movie uses its own language or region                                                    | Turns it off, so your default applies                                                                          |
| Use Custom Search                        | The show uses its own search engine (the **Custom Search** tab)                                      | Turns it off, so your default search engine applies                                                            |
| Use default source provider              | The show or movie is set to one data source on its **Basics** tab, instead of following your default | Switches it to your default data source. This only works if the show or movie is already linked to that source |

### File and folder names

| Check                            | Listed when                                                                     | Fix Issue does this                                                                                                             |
| -------------------------------- | ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------- |
| Use Custom Episode Naming Format | A show uses its own episode filename format (the **Custom Episode Naming** tab) | Turns the custom format off. If renaming is on, the next scan renames the files to your standard format                         |
| Use Custom File Name Format      | A movie uses its own filename format (the **Custom File Naming** tab)           | Turns the custom format off. If renaming is on, the next scan renames the file                                                  |
| Use custom folder name format    | A movie uses its own folder name format                                         | Turns it off and **renames the movie's folder** straight away. Stops with an error if a folder with the new name already exists |
| Movie Folder Format              | A movie's folder layout differs from your default                               | Sets it back to your default                                                                                                    |

### Where files are kept

| Check                                                                    | Listed when                                                                                               | Fix Issue does this                                                                                                                                                                                        |
| ------------------------------------------------------------------------ | --------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Use Custom season Folder Name Format, Use Custom season subfolder Format | A show's season folders are named or arranged differently from your default. A show can appear under both | Sets them back to your default                                                                                                                                                                             |
| Use Manual season Folders for TV Show                                    | A show has manual season folders                                                                          | Removes the manual folders and uses automatic season folders. **Files are not moved**, so a later scan may want to move them                                                                               |
| Has an automatic base folder supplied                                    | Automatic season folders are on, but the show has **no** base folder                                      | Sets the base folder to your default show location, or inside your TV library folder if you have exactly one                                                                                               |
| Has an base folder that is a library folder                              | The show's base folder is a whole library folder, so its files sit loose at the top of the library        | Creates a folder for the show inside that library folder and **moves the show's video files into it** straight away                                                                                        |
| Use Default folder supplied                                              | A movie uses automatic folders but has **no** base folder                                                 | Sets it to your movie library folder, if you have exactly one                                                                                                                                              |
| Use either manual or automatic folders                                   | A movie uses neither                                                                                      | Turns automatic folders on, if that is your default for new movies. Otherwise you need to set the folder yourself with **Edit Movie**                                                                      |
| Use manual folders                                                       | A movie uses a manual folder                                                                              | Switches the movie to its automatic folder and **moves its files there** straight away. Stops with an error if the movie has more than one manual folder or the automatic folder already holds video files |
| Manual Movie Folders Mirror Automatic                                    | A manual folder is the same as the automatic one                                                          | Removes the duplicate from the movie's settings                                                                                                                                                            |
| Movie has missing or empty manual folder                                 | A manual folder no longer exists or is empty                                                              | Removes it from the movie's settings and **deletes the empty folder**                                                                                                                                      |

## Fixing items

Right-click an item to see:

* **Force Refresh**: download the show's or movie's information again.
* **Edit TV Show** or **Edit Movie**: open its settings and change them yourself.
* **Visit** (movies only): open each of the movie's folders.
* **Fix Issue**: apply the fix described above.

To fix several at once, select them and right-click for **Fix Issues**. A progress window shows each fix as it runs. Fixed items drop off the list; any that could not be fixed stay, with the reason in the **Error Text** column.

{% hint style="danger" %}
**Fixes happen straight away.** They do not go to the Scan tab for you to approve first, and TV Rename cannot undo them. Four fixes change files on disk:

* **Has an base folder that is a library folder** moves files.
* **Use manual folders** moves files.
* **Use custom folder name format** renames a folder.
* **Movie has missing or empty manual folder** deletes empty folders.

Fix these one at a time and check the result before moving on.
{% endhint %}
