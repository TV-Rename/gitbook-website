# Organising

While the main objective of TV Rename is to rename and move/copy files into the appropriate locations in the library, there are many other things it can do at the same time:

### Keep Files Together <a href="#keep-files-together" id="keep-files-together"></a>

The system will keep files that share the same name together, renaming them all as one. This keeps related files (images, information, metadata) joined together. The system can also be configured to keep language specific files together for when you have subtitles in multiple languages.

{% hint style="info" %}
Further information can be found [**here**](../../menu/preferences.md#the-files-and-folders-tab).
{% endhint %}

### File Update Timestamp <a href="#file-update-timestamp" id="file-update-timestamp"></a>

The system can also be requested to update the ‘last updated’ dates to match the air-dates. This aims to help DNLA systems, but be wary if you are using a Linux based system such as a NAS for your media library. Linux has an inception date of 01/01/1970 and does not support earlier dates.

### DVD vs Aired Order <a href="#dvd-vs-aired-order" id="dvd-vs-aired-order"></a>

TV Rename can order a series in 2 ways at present:

* Aired Season Order
* DVD Season Order

To show how these are different take a look at Futurama on [The TVDB](http://thetvdb.com/series/futurama) and you can see that the episode order on DVD does not match the Aired order.

**Future Ideas**

There are a few ideas on the ideas wall to allow the ordering to be adjusted further to account for shows such as Mythbusters and American Dad. In both these cases the order that users want to organise the files does not match either the Aired or the DVD order

* [**Allow reorganising season numbers**](https://github.com/TV-Rename/tvrename/issues/67)
* [**Allow offset for episode numbers**](http://ideas.theideawall.com/TVRename/Forum/TopicDetails/ccf342c0-94b0-42f2-a0ba-a7cda261b2fa)

### Media Centres <a href="#media-centres" id="media-centres"></a>

In addition to renaming and moving files the system can also download/create files for various media players:

* Kodi
* Mede8er
* pyTivo
* WD TV Live Media Player
* others

In each case then the following types of files can be downloaded

* Fanarts, banners and posters
* Episode screenshots
* XML/Text files to explain details about the show/series/episodes

{% hint style="info" %}
Further information on the settings needed are [here](../../menu/preferences.md#the-media-centers-tab)
{% endhint %}

**Future Ideas**

There are plans to add support for other media centres and provide additional information by analysing the video files in more detail:

* [**Get the codec, size etc and use to show images in the show guide**.](https://github.com/TV-Rename/tvrename/issues/1040)
* [**AtomicParsley/MKVPropEdit support**](https://github.com/TV-Rename/tvrename/issues/1041)
* [**Support for additional Media Centres**](https://github.com/TV-Rename/tvrename/issues/1042)
