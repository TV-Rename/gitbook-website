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

TV Rename uses the Microsoft .NET 10 language. When the app loads it will check for its presence and let you know if any action is needed. It’s a free download from [Microsoft](https://www.microsoft.com/net/download/windows).

#### C++

The app will check on this and ask the user to upgrade if it's missing. It's needed as a dependency for CEF Framework
