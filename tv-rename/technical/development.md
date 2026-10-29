---
description: Details of the way that TV Rename is written and developed
---

# Development

### Source Code <a href="#source-code" id="source-code"></a>

You can find TV Rename’s source code (along with executables and this website) in [The TV Rename GitHub Repository](https://github.com/TV-Rename/tvrename).

### Development Links <a href="#development-links" id="development-links"></a>

* You can find the Developers Wiki [here](https://github.com/TV-Rename/tvrename/wiki)…
* For the longer term you can visit the “[Roadmap](https://github.com/TV-Rename/tvrename/milestones?direction=asc\&sort=due_date\&state=open)” which lists the proposed Milestones (a high level view of what's planned for when).
* In addition there is a [Developers Forum in Google Groups](https://groups.google.com/forum/#!forum/tv-rename-development) which you can request access to.
* The legacy forum can be [accessed](http://old.tvrename.com/bbold/) in read-only mode for background and history about the project

### Frameworks <a href="#framework" id="framework"></a>

#### Winforms C# application

#### .NET 10

TV Rename runs on the Microsoft .NET 10 Desktop Runtime. The installer doesn’t include it; if it isn’t on your PC, Windows tells you when you start TV Rename. It’s a free download from [Microsoft](https://dotnet.microsoft.com/en-us/download/dotnet/10.0).

#### C++

TV Rename needs the Microsoft Visual C++ Redistributable (v14, 2017 or newer) for the built-in browser it uses to show information (the CEF Framework). The app checks for it and, if it's missing, downloads the installer for you.
