# Remove Shows With No Folders

**Remove Shows With No Folders** tidies TV Rename's library by removing TV shows and movies whose folders no longer exist on disk, for example shows you have finished and deleted.

It only changes TV Rename's own list. **No files or folders are deleted.**

A progress window checks the library, then the **Scan** tab opens with each show or movie to be removed listed under **Remove from library**. Untick any you want to keep, then click `Do Checked`.

A TV show is proposed for removal only when all of these are true:

* at least one of its episodes has aired,
* none of the folders TV Rename expects for it exist, and
* its base folder doesn't exist either. A show whose base folder is still there, even if it is empty, is kept.

A movie is proposed when it has been released and none of its folders exist.

Shows that haven't started airing and movies that haven't been released are never proposed, as you wouldn't have any files for them yet.

{% hint style="info" %}
If you remove something by mistake, add it again. Anything you had customised for it, such as a custom name or ignored seasons, will need setting again.
{% endhint %}
