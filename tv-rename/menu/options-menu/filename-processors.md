# Filename Processors

![](https://www.tvrename.com/assets/images/options/filename-processors-01.png)

In much the same way that the _**Filename Template Editor**_ is used to process the names of files being moved to the media library so _**Filename Processors**_ is used to inform TV Rename what filenames to look out for when searching for a missing files

To really understand the contents of the Regex column above, you need a working knowledge of [Regular Expressions](https://regexone.com/).

Once you have figured out whats going on you can see that all the regular expressions capture the season and episode number of a show from the filename. Each one can work on just the filename: -

> ShowName S01E07.avi

or on the whole path: -

> C:/files/ShowName/S01E07.avi

The expressions are evaluated in order (top down).

Each expression can be toggled on and off, as can the ability to process a full path.

Each expression has a Notes field which can be used to remind the user why the expression was added.

Additionally, a folder can be specified to test the results of the Regular Expression.

If a match is found during the test the matching expression is indicated.

In all likelihood you will find it unnecessary to make changes here, only if a new, totally unrecognisable file name structure appeared would it be necessary, and then there would probably be discussion about it in the forum.
