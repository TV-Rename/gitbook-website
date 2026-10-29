# Search Engines

**Options>TV Show Search Engines** and **Options>Movie Search Engines** each open a _Modify Search Engines_ window, one for TV shows and one for movies. These control TV Rename’s outgoing interface with the world (other than its data sources). Here, you can configure how and where TV Rename points a web browser searching for files.

<figure><img src="../../.gitbook/assets/image (70).png" alt=""><figcaption></figcaption></figure>

Using the `Add` and `Delete` buttons you can create or remove records at will, and the `Tags...` pop up a list of supported tags to remind you whats available. (The tags supported are the same as those listed in the [Filename Template Editor](filename-template-editor.md).)

TV Rename starts with three entries in each list: Google, YouTube and Vimeo. As an example, here is the TV show URL entry for Google.

> https://www.google.com/search?q={ShowName}+S{Season:2}E{Episode}

The list of URL’s can be used from the _**Scan**_ and _**Schedule**_ tabs. The last used entry becomes the default, and its name appears on a search button on the toolbar (to the right of the `Refresh` button on the Schedule tab). It can be changed by clicking the `▼` button next to it and selecting another entry.

With a little ingenuity you can get really creative with these entries and pass your search to its specific target through a web proxy.
