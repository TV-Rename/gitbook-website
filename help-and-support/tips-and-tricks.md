# Tips & Tricks

### Tips from the developers <a href="#tips-from-the-developers" id="tips-from-the-developers"></a>

* Most items can be double-clicked, to do the most “useful” thing for them.
* Folders, shows, and episodes can be right-clicked for menus of appropriate actions.
* Column headers can be clicked to sort by that column.
* Folder lists support “dragging and dropping” folders from Explorer.
* You can remove items from the finding, renaming and organising lists by selecting them, and pressing “Delete” on your keyboard.
* Selecting one of the main tabs by double-clicking will automatically do the “Find”, “Check”, or “Refresh” action associated with that tab.
* Changes you make are not saved unless you specifically do so. TV Rename will prompt you to save when you exit (if it needs to). If you screw something up, just exit without saving and TV Rename will forget everything you have done since the last save when it is reloaded.
* TV Rename stores all its data in JSON files. For more information on what there is, and where it is read the [Technical Guide - Configuration Files](../the-manual/technical-guide/logs-and-configuration.md).
* A number of TV Rename’s functions can be accessed using the command line. You can find more details [here…](../the-manual/command-line.md).
* Whatever manipulation TV Rename applies to your files, it will never change the season or episode number of a show. Even if the show and episode names get corrupted the season and episode numbers will remain unchanged. This means that the problem should be fixable after changing some settings, or adding new rules. At least, that’s the theory.&#x20;

### Tips from our users <a href="#tips-from-our-users" id="tips-from-our-users"></a>

{% hint style="success" %}
If your media library uses removable media to store files the assigned drive letter changing each time a usb device is plugged in can be a real pain.

A small tweak in Windows settings will “fix” the drive letter for the device in question.

There are numerous internet guides for doing this, the following link will get you started:&#x20;

[**Google - fix usb drive letter assignment**](https://www.google.co.uk/search?q=fix+usb+drive+letter+assignment)

_**Andy B**_
{% endhint %}

{% hint style="success" %}
You can change the behaviour of some earlier versions of Windows 10 regarding mapped drives. In the registry under:

**HKEY\_LOCAL\_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\Policies\System**

Create a new **DWORD (32 Bit)** named **EnableLinkedConnections** and set the value to **“1”**.

Restart Windows after making the change. All applications should now see the same mappings regardless of being in User or Admin mode.

_**Jürgen**_
{% endhint %}

{% hint style="info" %}
_**Windows 7 - SSL issue**_

_**Some Win 7 systems have issues connecting to TVDB v4 API**_

[https://groups.google.com/g/tvrename/c/\_w9CwFeM8fs/m/qU56rmBkAQAJ](https://groups.google.com/g/tvrename/c/\_w9CwFeM8fs/m/qU56rmBkAQAJ)

Confirm that KB3042058 & KB3020369 are installed. &#x20;

Add the missing registry keys for "TLS 1.2" under **HKEY\_LOCAL\_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols**\
Which is beautifully documented here\
[https://manage.accuwebhosting.com/knowledgebase/3008/how-do-i-enable-tls-1-2-on-windows-7.html](https://manage.accuwebhosting.com/knowledgebase/3008/how-do-i-enable-tls-1-2-on-windows-7.html)

_**Don**_&#x20;
{% endhint %}

{% hint style="info" %}
_**High DPI issue resolution**_

__[_https://groups.google.com/g/tvrename/c/oAvxJxpBW6g/m/huoHHgmIAgAJ_](https://groups.google.com/g/tvrename/c/oAvxJxpBW6g/m/huoHHgmIAgAJ)__

__[_https://groups.google.com/g/tvrename/c/5WjHfCwFLIU/m/9Fb5iywbDQAJ_](https://groups.google.com/g/tvrename/c/5WjHfCwFLIU/m/9Fb5iywbDQAJ)__

Changing the high DPI compatibility settings for the shortcut works

[https://groups.google.com/g/tvrename/c/LV47f\_md73I](https://groups.google.com/g/tvrename/c/LV47f\_md73I)

_**Michael**_
{% endhint %}
