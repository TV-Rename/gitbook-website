# TV Show Configuration

### Add/Edit Show <a href="#addedit-show" id="addedit-show"></a>

The _Add/Edit Show_ window has a number of tabs of its own, they are discussed below: -

#### The Basics Tab <a href="#the-basics-tab" id="the-basics-tab"></a>

![Add/Edit Show - The Basics Tab](https://www.tvrename.com/assets/images/main-window/add-edit-show-basics-01.png)

The “Basics” Tab is the starting point for telling TV Rename about a show you which to monitor.

The best way to illustrate this is with an example so lets add a show called “The Good Doctor” to TV Rename.

The first step is to tell TV Rename about the show. If you know it you can enter TheTVDB’s code for the show, otherwise type the shows name (e.g. “the good doctor”) and click on `Search`.

TV Rename ![Add/Edit Show - Search Results](https://www.tvrename.com/assets/images/main-window/add-edit-show-basics-02.png)will search for matches to your entry in TheTVDB’s database, cache the results locally and display the matches. The search also works with partial show names. For example you could search for just “doctor”, but “doctor” being fairly common in TV show titles, returns over 80 results (including ours!), and you will have to delve into the list to find the one you want. Once you have found the correct show, click on it to highlight it.

If all you want to do is see the details of the show then you’re done! Just click `OK` at the bottom of the window and TV Rename will pull the necessary data from [The TVDB](http://thetvdb.com) to populate the _**My Shows**_ tab.

Once the update is complete _**My Shows**_ includes “The Good Doctor” and looks like this: -

![My Shows - New Show Added](https://www.tvrename.com/assets/images/main-window/my-shows-02.png)

All the Show and Season information is downloaded and the _**When to Watch**_ tab will now list any future episode dates, but there are no links to the media library.

Lets go back and tweak “The Good Doctor”. Assuming the show is listed in _**My Shows**_, make sure it is highlighted and click `Edit` to recall the partially populated _Add/Edit Show_. If it isn’t listed in _**My Shows**_ follow the steps above to get the show name populated and then carry on as described below.

The “Custom show name:” field allows you to change the show name in both TV Rename and the media library (except the base folder). You may like to remove “The” from names, or change extra information like the year the show was originally produced that appears with some shows. If you tick the box and enter a new name in the field provided the shows title will be replaced with this entry.

The “Airs in Timezone:” drop-down tells TV Rename that the air time from [The TVDB](http://thetvdb.com) is in that specific timezone. Most shows are in Eastern USA time, but British shows (e.g. Maigret) will be in British Standard Time. This only has an effect in the _**When to Watch**_ tab which translates these times into your local timezone, or in the status bar when calculating time till the “Next Airing:”.

_Default:_ _**Eastern Standard Time**_

If you wish to ignore specific seasons of a show enter the season numbers (space separated) in the “Ignore Seasons:” field (Entering a “0” will ignore “Specials”).

_Default:_ _**Empty Field**_

New in Version 2.6 the “Custom Language:” tick box and drop-down allows you to set a “non-default” language for the show in question. To activate it simply tick the box and select the preferred language for the show from the drop-down.

_Default:_ _**Un-ticked**_

To complete the minimum setup for adding the show to the library we now need to go to the [“Folders” Tab](https://www.tvrename.com/manual/user/#the-folders-tab).

[Return to Top](https://www.tvrename.com/manual/user/)

#### The Advanced Tab <a href="#the-advanced-tab" id="the-advanced-tab"></a>

![The Advanced Tab](https://www.tvrename.com/assets/images/main-window/add-edit-show-advanced-01.png)Here, you can further manipulate the way data from [The TVDB](http://thetvdb.com) is handled as it is merged into the local data.

The “Use DVD order” tick box comes into play when the episodes aired on TV in a different order to those presented on the DVD. [The TVDB](http://thetvdb.com) usually has details of these orders and this tick box allows you to choose your preference for the current show. A Really good example of this is the 1967 ITV show [“The Prisoner”](https://www.thetvdb.com/?tab=season\&seriesid=74805\&seasonid=8058\&lid=7), which, whilst it was written as one season of seventeen episodes still causes as much controversy (and argument) over it’s running order today as it did when it was originally released.

The “Show next airdate in When to Watch” tick box toggles the display of the shows “Future” and “Later” episodes in the _**When to Watch**_ tab.

The “Specials count as episodes” tick box is useful with shows such as “Mythbusters” where specials are often counted as normal episodes.

The “Do Renaming” tick box tells TV Rename to use the names built using the [_**Options>Filename Template Editor**_](https://www.tvrename.com/manual/options#filename-template-editor) when copying or moving files if it is ticked, otherwise they will be left unchanged.

The “Do missing check” tick-box enables or disables the ability to check for missing episodes, if the option is ticked some degree of granularity is provided by the “Include future episodes” and “Include no airdate” tick-boxes.

“Use sequential number matching” will match episodes based on their overall airing order. Because this can cause a large number of false matches, the box is un-ticked by default.

For example, Season 4 Episode 9 of Marvel’s Agents of S.H.I.E.L.D. is the 75th episode aired, so with this option enabled “Marvel’s Agents of S.H.I.E.L.D. - 75 - Broken Promises.mkv” will be seen at S04E09.

The “Manual/Additional Folders” section allows you to manually add and remove additional Seasons and associated folders.

[Return to Top](https://www.tvrename.com/manual/user/)

#### The Show Aliases Tab <a href="#the-show-aliases-tab" id="the-show-aliases-tab"></a>

![The Show Aliases tab](https://www.tvrename.com/assets/images/main-window/add-edit-show-aliases-01.png)The Show Aliases tab only affects source files, it does **not** affect show episodes in your media library (TV Rename can work out the correct name for a file in the library from the containing folder structure and the show/season number).

Sources often rename files because of the excessive length of the shows name, for example “Law and Order- Special Victims Unit” could be represented as “L\&O-SVU”. Adding “L\&O-SVU” as an alias would cause any source file with that abbreviated name be renamed correctly when moved or copied into the library.

Another good example (though for different reasons) would be the BBC1 show “Doctor Who”, [The TVDB](http://thetvdb.com) correctly calls it “Doctor Who” which TV Rename will recognise, however some sources variously call the show “Dr. Who” or “Dr Who” causing some confusion. Adding “Dr. Who” and “Dr Who” as aliases for “Doctor Who” will fix this problem and everything will be correctly named “Doctor Who” when moved or copied into the library.

[Return to Top](https://www.tvrename.com/manual/user/)

#### The Search Tab <a href="#the-search-tab" id="the-search-tab"></a>

![The Search Tab](https://www.tvrename.com/assets/images/main-window/add-edit-show-search-01.png)The Search Tab allows you to create a custom search for files on a per show basis.

This is useful if you collect episodes of a show that falls outside the scope of the “general” search engines and has its own genre-specific sites and searches (Japanese Anime for example).

Using the same technique and tag structure as found in the [Options>Search Engines](https://www.tvrename.com/manual/options#search-engines) tab you can create a search specific to the show without affecting the “general” searches.

This option is disabled by default but it can be enabled for the specific show by ticking the “Use Custom Search” box in the tab.

[Return to Top](https://www.tvrename.com/manual/user/)

#### The Folders Tab <a href="#the-folders-tab" id="the-folders-tab"></a>

![Add/Edit Show - Folders](https://www.tvrename.com/assets/images/main-window/add-edit-folders-01.png)

Completing the “Folders” Tab tells TV Rename about the library folder for the show. Returning to our example of “The Good Doctor”: -

If the “Automatic Folders” box is ticked the path to the base folder can be typed in the text box or filled in by browsing, but either way, now TV Rename knows the location of the shows base folder in the media library all the “really useful” stuff can begin!

The three radio buttons determine how the seasons of the show are handled: -

Selecting “Library Default” will tell TV Rename to create a sub folder for each season, naming them “Season 1”, “Season 2”, “Season 3” etc.

Selecting “Base Folder” will tell TV Rename to store all the related files in the base folder specified previously.

Selecting “Custom Pattern” allows you to specify (using text and tags) the naming of the season folders.

| _**Default:**_ | “Library Default” | _**Selected**_ |
| -------------- | ----------------- | -------------- |

If you require more granular control you can un-tick the “Automatic Folders” option and use the “Manual/Additional Folders” entries to specify the exact name and location for each season folder used by the show.

[Return to Top](https://www.tvrename.com/manual/user/)

### Auto Add Shows <a href="#auto-add-shows" id="auto-add-shows"></a>

Whilst discussing “Add/Edit Shows” it would be remiss not to mention “Auto Add Shows”.

This not-so-obvious trick in TV Rename’s functionality attempts to add video files that have been downloaded but are unknown to TV Rename to its database for inclusion in the library.

It is activated by ticking the “Notify when new shows are found” box in the [Options>Preferences Bulk/Auto Add](https://www.tvrename.com/manual/options#the-bulk--auto-add-tab) window.

For example: -

If the show file “Westworld.S01E01.HDTV.x264.mp4” exists in the downloads directory but **not** in TV Rename’s database and the “Notify when new shows are found” box is ticked; a scan will result in the following pop-up appearing…

![New Show Detected...](https://www.tvrename.com/assets/images/main-window/new-show-detected-01.png)

TV Rename has taken it upon itself to attempt to find the show name and look it up using [The TVDB](http://thetvdb.com)!

You now have a number of options: -

Selecting `Skip Auto Add` stops doing auto add for this scan for all files.

Selecting `Ignore File Forever` stops doing auto add on that file for this (and all future) scans.

Selecting `Leave for later` ignores this file for this scan.

However, if you select the matching series name in the central window (in this case “Westworld”) the “Location:” will be modified to include the show name. Click `Quick Add` and the file will be added to the library, prompting you to create the required sub-directories as necessary.

Auto Add uses the default settings for almost all options (so the timezone etc. may be need adjusting).

The locations used are based on those entered as part of “Bulk Add”.

[Return to Top](https://www.tvrename.com/manual/user/)

### Edit Season Rules <a href="#edit-season-rules" id="edit-season-rules"></a>

The “Edit Season Rules” pane allows you to manipulate the local data from [The TVDB](http://thetvdb.com) to suit your episode structure.

![Edit Season Rules](https://www.tvrename.com/assets/images/main-window/edit-season-rules-01.png)

Episodes 1 and 2 of Season 5 of “Marvel’s Agents of S.H.I.E.L.D.” aired as a double episode so only one file exists, however [The TVDB](http://thetvdb.com) correctly has both episodes listed individually, so there is a conflict.

The image illustrates a rule that merges the two episodes into one. This will affect the name displayed in the _**My Shows**_ tab, and the naming of the file in the media library.

The rules are applied in top to bottom order, you can use the the `Up` and `Down` buttons to move a rule.

`Add`, `Edit`, and `Delete` will manipulate the list as expected.

![Add/Modify Rule](https://www.tvrename.com/assets/images/main-window/add-modify-rule-01.png)Clicking either `Add` or `Edit` will open the _Add/Modify Rule_ pane. The only difference being `Add` allows you to create a new rule and `Edit` pulls in the data from a highlighted rule for you to change.

In this example we are editing the rule shown above. This is a two part process, firstly select an “Action:”, and secondly tell TV Rename what to apply the action to.

In this case the “Action” is “Merge”, we are merging “1” and “2” i.e. Episodes 1 and 2 of the selected season, And we will let TV Rename name the new file automatically.

The “Actions:” available are: -

| **Ignore** | Keep the specified episode in the guide, but don’t check for it (or rename it) on disk locally.   |
| ---------- | ------------------------------------------------------------------------------------------------- |
| **Rename** | Manually set the name of an episode.                                                              |
| **Remove** | Make a an episode disappear. All episodes above will be renumbered down to fill the gap.          |
| **Swap**   | Swap the position of two episodes.                                                                |
| **Merge**  | The episodes numbers supplied all in a single multi-episode file.                                 |
| **Insert** | Manually add an episode into the season. Later episodes are renumbered to accommodate the change. |
| **Split**  | Turn one episode into many. Following episodes are renumbered to accommodate the change.          |

After applying a rule, go to _**My Shows**_ , select the show, and click `Refresh`. You will then see (and can check) the effects of the rules you’ve created.
