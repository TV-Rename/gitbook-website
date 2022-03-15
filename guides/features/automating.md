# Automating

TV Rename aims to do as much as it can to automate the storage of media files. To make the process as automated as possible it can:

* _Auto Add shows_ – see ‘Automated Addition’ above.
* _Auto folder creation_ – TV Rename can be setup via preferences [(**here**)](https://www.tvrename.com/manual/options#the-scan-options-tab) to automatically create folders for shows and series. This will create based on the defaults.
* _Auto folder & file deletion_ – TV Rename can identify files and folders that can be removed and then get rid of them.
  * _‘Delete Empty Folders after moving Files’_ - Review Folders as movie files are copied out of the folder. Sometimes files are downloaded with many accompanying files which are not needed. If this is the case then this function can clean up the unused files. [**It is configured here**](https://www.tvrename.com/manual/options#the-folder-deleting-tab).
  * _‘Clean-Up’_ - Files and folders in the download directory that match episodes already in the library. This is useful when something else keeps hold of the lock on the files and they cannot be removed after the move operation, but occasionally deletes ‘PROPER’ or improved files that are improvements to what is already in the library. [**It is setup here**](https://www.tvrename.com/manual/options#the-folder-deleting-tab).
  * Suggest recycling files/folders rather than deleting [**as specified here**](https://www.tvrename.com/manual/options#the-folder-deleting-tab).
* _Multi-episode Merging_
  * Proactive. In the settings (here) TV Rename can be pro-actively setup to create merge rules. If a downloaded or library file matches a multi episode file [(**see here**)](https://www.tvrename.com/manual/options/#the-scan-options-tab) then it will automatically create a merge rule.
  * Reactive. Under the beta option, ‘Duplicate finder’ will scan the library and look for files that look like they are multi-episode files based on a few criteria:
    * The two(or more) episodes have the same air-date
    * The episodes name is similar.
    * One or more of the episodes are missing.
    * The file that is on disk is larger than normal which would indicate that there is more than one episode in the file.
* _Auto-update_
  * On start-up TV Rename will check to see whether it is on the latest version and suggest that it is updated if not.
  * From “Help” in the menu bar you can manually check for an update.
* _Auto Scanning_
  * As files change or on a fixed period (set in [**Options>Settings Search Folders**](https://www.tvrename.com/manual/options#the-search-folders-tab)).
* _Auto Upgrades_
  * As better quality files are identified then they are used to replace lesser quality versions.
