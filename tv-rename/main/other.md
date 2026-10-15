# Other

## The Status Bar

The status bar runs along the bottom of the main window.

On the left it shows the next episode due to air from the shows in your library, how long until it airs, and the day and time it airs, for example:

`Next airing: Judy Justice.S04E111, 0d 10h (Mon, 4:00 AM)`

Here the episode airs in 0 days and 10 hours, on Monday at 4:00 AM in your own time zone. If nothing is due to air it shows `Next airing: ---`.

On the right it shows what TV Rename is doing with the data sources (TheTVDB, TMDB and TVmaze):

* While TV Rename is downloading show and movie information, it shows what is being downloaded, with a progress bar. See [Automatic Background Download](../menu/options-menu/automatic-background-download.md).
* When [Offline Operation](../menu/options-menu/offline-operation.md) is turned on, it shows `OFFLINE`.
* Otherwise it is blank.

## Upcoming

If **Show notification area icon** is ticked in [Preferences > Display](../menu/preferences.md#the-display-tab), TV Rename puts its icon in the Windows notification area, at the right-hand end of the taskbar. If you can't see the icon, look under the hidden icons arrow (`^`).

* **Click the icon once** to see the **Upcoming Shows** window. It lists the next five episodes due to air, each with how long until it airs, the day, the time and the episode. It appears in the bottom-right corner of your main screen and closes itself after about 10 seconds.
* **Double-click the icon** to bring the main TV Rename window to the front.

## Update Available...

TV Rename can check for new versions of itself. How often it checks is set on the **App Updates** tab of [Preferences](../menu/preferences.md): tick **Check for Updates**, then choose **on every start** or **at certain intervals**.

When a newer version is found, an **Update Available...** button appears at the top right of the main window. Unless **No dialog when an update is available** is ticked on the App Updates tab, the **Available Update** window also opens.

Clicking **Update Available...** checks again and opens the **Available Update** window, whether or not that option is ticked. The window shows the release notes for the new version and these buttons:

| Button                    | What it does                                                                                       |
| ------------------------- | -------------------------------------------------------------------------------------------------- |
| **Download Now**          | Opens the download for the new version in your web browser.                                        |
| **View Release Notes**    | Opens the release notes in your web browser.                                                       |
| **Download Now and Quit** | Opens the download for the new version in your web browser and closes TV Rename, ready to install. |
| **Cancel**                | Closes the window.                                                                                 |

You can also check at any time with **Help > Check For New Version**. If you already have the latest version you will see "There is no update available please try again later."

{% hint style="info" %}
When **Mode** is set to **Beta** in [Preferences > General](../menu/preferences.md#the-general-tab), TV Rename offers beta versions as well as normal releases.
{% endhint %}
