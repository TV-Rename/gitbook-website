# Filename Processors

<figure><img src="../../.gitbook/assets/image (71).png" alt=""><figcaption></figcaption></figure>

In much the same way that the _**Filename Template Editor**_ is used to process the names of files being moved to the media library so _**Filename Processors**_ is used to inform TV Rename what filenames to look out for when searching for a missing files

To really understand the contents of the Regex column above, you need a working knowledge of [Regular Expressions](https://regexone.com/).

Once you have figured out whats going on you can see that all the regular expressions capture the season and episode number of a show from the filename. Each one can work on just the filename: -

> ShowName S01E07.avi

or on the whole path: -

> C:/files/ShowName/S01E07.avi

The expressions are evaluated in order (top down). Use `Move Up` and `Move Down` to change the order, `Add` and `Delete` to add or remove an expression, and `Defaults` to put back the original list (TV Rename asks you to confirm first).

Each expression can be toggled on and off (**Enabled**), as can the ability to process a full path (**Full Path**).

Each expression has a Notes field which can be used to remind the user why the expression was added.

The bottom of the window lets you test the expressions. Choose what to test against:

* **Test Folder:** – the files in a folder you pick with `Browse...`.
* **Torrent Queue** – the files your torrent program is currently downloading.
* **Text:** – a file name you type in.

**Show:** sets the show to test against. Tick **Test All** to test every expression; otherwise only the expressions selected in the list above are tested.

For each file the results show the **Filename**, the **Show(s)**, the **Season** and **Episode** found, and the **Rule** (expression) that matched.

In all likelihood you will find it unnecessary to make changes here, only if a new, totally unrecognisable file name structure appeared would it be necessary, and then there would probably be discussion about it in the forum.
