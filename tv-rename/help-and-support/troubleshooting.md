---
description: Some common problems (and their solutions)
---

# Troubleshooting

### Errors after installing -> Check dependencies <a href="#check-dependencies" id="check-dependencies"></a>

1. Install TV Rename
2. TV Rename needs the .NET 10 Desktop Runtime. The installer doesn't include it; if it isn't on your PC, Windows tells you when you start TV Rename.
   1. Download it from [https://dotnet.microsoft.com/en-us/download/dotnet/10.0](https://dotnet.microsoft.com/en-us/download/dotnet/10.0)
3. Visual C++ [Redistributable ](https://learn.microsoft.com/en-us/cpp/windows/latest-supported-vc-redist?view=msvc-170#visual-studio-2015-2017-2019-and-2022)(v14, 2017 or newer). If it's missing, TV Rename downloads the installer for you.

{% hint style="info" %}
Help > Browser Test will verify that all C++ dependencies are found
{% endhint %}

### Issues with out of date show information -> Repair Corrupt Data <a href="#repairing-corrupt-data" id="repairing-corrupt-data"></a>

Occasionally information for shows gets corrupted and needs refreshing. The quickest way to do this is a “Forced Refresh”, which comes in two flavours.

#### Refresh Show

Firstly, if the problem is small, only effecting a small number of shows, right clicking a problematic show on the _**TV Shows**_ tab will pop up a menu on which one of the options is “Force Refresh”. Clicking this option will tell TV Rename to go to the show's data source and re-collect all the data available for that show and re-populate the local cache. This will often fix the issue.

The second solution is far more drastic in its effect.

#### Force Refresh All

“Force Refresh All” in the **Tools** menu is the “Tool of Last Resort”. If TV Rename’s representation of your media library is a real mess or the previous solution doesn’t help then this is your only real alternative.

**READ THE WARNING CAREFULLY AND PAY ATTENTION**. If you click `Yes` there’s no going back, all the information TV Rename has stored from TheTVDB, TMDB and TVmaze is **DELETED** and has to be downloaded again. See [Force Refresh All](../menu/tools-menu/force-refresh-all.md) for what happens next. (Now might be a good time for a coffee, if your library is large and internet connection slow it may take a while!)
