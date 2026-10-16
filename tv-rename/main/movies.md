---
description: TV Rename also managed movies...
---

# Movies

## Movie Library

<figure><img src="../.gitbook/assets/image (26).png" alt=""><figcaption></figcaption></figure>

Below these panels are a series of buttons which allow you to manage the content. They are: -

* `Add` - Adds a new movie to the list. Remember you may need to add folders to for the movie separately if you need to monitor it in the media library.
* `Edit` - Edit the currently selected movie
* `Delete` - Remove the currently selected movie(s) from TV Rename’s database, and optionally delete the selected movie(s) from the media library - _**careful!**_
* `Refresh` - Refresh the current view
* `Scan Movies` - Do a scan just for Movies (ie no TV Shows)
* `Filter` - Filter the listed shows based on the entered criteria.

The right hand side of the screen has 3 tabs:

* **Information** - key information about the movie. NB you can expand the Cast and Crew section to get more information
* **Images** - Any downloaded images and posters from the movie
* **Trailer** - Embedded youtube viewer of the movie's trailer

**REMEMBER:**

* Clicking on the `Add` button will open the _Add/Edit Movie_ window ready to add another show.
* Clicking the `Edit` button with a **show** highlighted will open the same window pre-populated with that shows details.
* Right-clicking on a movie will give you some custom options too, including
  * `Force Refresh` - Force TV Rename to delete the cached data it has about that movie and refresh from the source
  * `Scan Movie`- Do a scan just for this movie.

### Filters

<figure><img src="../.gitbook/assets/image (32).png" alt=""><figcaption></figcaption></figure>

Allows you to filter the movie list to just the ones you are interested in at that moment

### Adding Movies to the library

There are a number of ways one can add movies to their library:

1. Manually
2. Use 'Scan Movie Folder'. This is useful if you have a selection of movies in a folder and you wish to orgnise them into your library. This will iterate through the movie files in the specified folder and:
   1. If the file matches movie in your library ask whether it is a new movie, or it should replace the existing movie file
   2. If the file does not match a movie in your library, but does match one on TMDB, offer to add the movie and copy the file into the correct place
   3. if it's not sure ask you what to do with the file
3. If you already have an orgnised movie library, use bulk add to keep the current directory structure and add all movies to the library.
4. Copy movie files into the search folder. Enable 'Auto-add' and then run a scan. Auto add will identify that the file is new and ask to add the new movie to the library.

## Add/Edit Movie

### Basics

<figure><img src="../.gitbook/assets/image (27).png" alt=""><figcaption></figcaption></figure>

The Basics tab links the movie to its entry at the data source and sets what the movie is called.

To find the movie, type its name (or its code at the source, if you know it) in the code box and click `Search`, then click the right movie in the list of matches.

* **Source** – where TV Rename gets this movie’s information. **Library Default** uses the **Default Movie Source** on the [Data Sources](../menu/preferences.md#data-sources) tab of **Options>Preferences**. **The TVDB** or **TMDB** uses that source for this movie only.
* **Custom show name** – tick it and type a name to use instead of the title from the source. TV Rename uses this name for the movie everywhere, including its folder and file names.
* **Custom Language** – tick it and choose the language to ask the source for, for this movie only.
* **Custom Region** – tick it and choose the region to use for this movie’s release date, instead of the **Preferred region** on the Data Sources tab.

### Folders

<figure><img src="../.gitbook/assets/image (28).png" alt=""><figcaption></figcaption></figure>

The Folders tab tells TV Rename where this movie’s files are kept in your library.

**Folder Type** sets how the movie is stored:

| Folder Type             | What it means                                                                                                             |
| ----------------------- | ------------------------------------------------------------------------------------------------------------------------- |
| Single Movie per Folder | The movie has a folder of its own.                                                                                        |
| Many Movies per Folder  | The movie’s file sits directly in the base folder, together with other movies.                                            |
| DVD format              | The folder holds a DVD copy of the movie. TV Rename looks for `VIDEO_TS\VIDEO_TS.IFO` in it and doesn’t rename the files. |
| Bluray format           | The folder holds a Blu-ray copy of the movie. TV Rename looks for `BDMV\index.bdmv` in it and doesn’t rename the files.   |

Tick **Automatic Folders** to let TV Rename work out the movie’s folder:

* **Base Folder** – the movie library folder the movie goes in. The list holds your **Movie Library Folders** from the [Library Folders](../menu/preferences.md#the-library-folders-tab) tab of **Options>Preferences**.
* **Movie Folder Name** – **Subdirectories (default)** names the movie’s folder with the **Folder format** on that same Library Folders tab, which is shown in grey beside it. **Custom Subdirectories** lets you type a different folder name for this movie; click `Tags...` to see the tags you can use.

Tick **Manual/Additional Folders** to list the movie’s folders yourself. Type a folder in **Folder:** (or click `Browse...` to pick one) and click `Add`. Select a folder in the list and click `Open` to open it in File Explorer, or `Remove` to take it off the list.

At least one of **Automatic Folders** and **Manual/Additional Folders** must be ticked.

If some files in these folders are on TV Rename’s ignore list, the tab says so and shows a `See Ignore List` button.

### Custom File Naming

By default TV Rename will name movie files using the [Filename Format](../menu/preferences.md#the-library-folders-tab) in **Preferences>Library Folders**. If this movie should use its own format then it can be overridden and specified here:

<figure><img src="../.gitbook/assets/image (29).png" alt=""><figcaption></figcaption></figure>

### Aliases

Aliases are other terms that TV Rename uses (as well as the main name of the media) to match a filename to the movie name. TV Rename has 2 types of aliases:

1. **Source Aliases** that come from the data source
2. **Custom Aliases** that the user adds manually

<figure><img src="../.gitbook/assets/image (30).png" alt=""><figcaption></figcaption></figure>

### Advanced

Use the advanced options to configure when and how the movie should be scanned and renamed.

<figure><img src="../.gitbook/assets/image (31).png" alt=""><figcaption></figcaption></figure>
