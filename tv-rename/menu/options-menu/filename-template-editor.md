# Filename Template Editor

<figure><img src="../../.gitbook/assets/image (69).png" alt=""><figcaption></figcaption></figure>

This is where the format of the filenames that TV Rename will rename to are defined.

To help illustrate the results the “Sample and Test:” panel contains the processed entries from the show and season selected in the _**My Shows**_ tab.

The “Naming template:” text box displays a tokenised version of the filename which can be edited directly or populated using the “Tags:” drop-down, or overwritten with a record selected from the “Presets:” drop-down. Any changes in the “Naming Template:” are automatically reflected in the “Sample and Test:” panel.

The available tags with their definitions are listed below: -

<table data-header-hidden data-search="false"><thead><tr><th width="187"></th><th></th></tr></thead><tbody><tr><td>{ShowName}</td><td>Name of the Show</td></tr><tr><td>{Season}</td><td>Number of the season</td></tr><tr><td>{Season:2}</td><td>Number of the season forced to 2 characters with a leading zero</td></tr><tr><td>{Episode}</td><td>Number of the episode (within a season), eg S01E03</td></tr><tr><td>{Episode2}</td><td>Number of the second episode of a pair (within a season), eg S01E04-E05<br>created by the default S{Season:2}E{Episode}[-E{Episode2}])</td></tr><tr><td>{EpisodeName}</td><td>Name of the Episode</td></tr><tr><td>{Number}</td><td>Overall number of the episode</td></tr><tr><td>{Number:2}</td><td>Overall number of the episode forced to 2 characters with a leading zero</td></tr><tr><td>{Number:3}</td><td>Overall number of the episode forced to 3 characters with leading zero(s)</td></tr><tr><td>{SeasonNumber}</td><td>Some season numbers do not start at 1, eg they may go 2012,2013,2014. {SeasonNumber} is the nth season, so would be 1,2,3 in this example</td></tr><tr><td>{SeasonNumber:2}</td><td>As above, but forced to 2 characters with a leading zero</td></tr><tr><td>{ShortDate}</td><td>Air date in short format, eg 25/12/2017</td></tr><tr><td>{LongDate}</td><td>Air date in lomg format, eg 25 December 2017</td></tr><tr><td>{YMDDate}</td><td>Air date in YMD format, eg 2017/12/25</td></tr><tr><td>{AllEpisodes}</td><td>All episodes - E01E02 etc</td></tr></tbody></table>

<table data-header-hidden><thead><tr><th width="119"></th><th></th></tr></thead><tbody><tr><td><em>Default:</em></td><td><em><strong>{ShowName} - S{Season:2}E{Episode}[-E{Episode2}] - {EpisodeName}</strong></em></td></tr><tr><td></td><td>(the second preset).</td></tr></tbody></table>
