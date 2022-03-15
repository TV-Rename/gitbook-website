# Adding Movies & TV Shows

TV Rename will track many TV Shows in your library. These can be added in 3 key ways:

* _Manually_ – Added manually by entering the name into the ‘Add Show’ screen from the main ‘My Shows’ tab
* _Bulk Add_ – TV Rename can scan through some specified folders (Monitor Folders) via the ‘Bulk Add’ tool. It will display a list of shows that are not already in the library and allow them to be added en-masse.
* _Automated_ – TV Rename can be setup to look at files in the download folder (Search Folders) and (if it can’t find an appropriate show in the library) offer the user some suggestions about which series/show to add to the library.

### **Manual Addition**

Manual addition is the simplest way of adding shows into the library. You can enter (and search for) the show by name or for more precise addition enter a TVDB Id. All the options about the show can be edited, but they key ones to add are:

* Directory location to store the location of the files for the series
* Time zone for the series (this is not available from TVDB, so must be entered manually)

### **Bulk Addition**

TV Rename can search through your library of existing (organised) files to find shows that are not in the library. This is initiated from the menu bar, with config options are in the preferences under ‘Bulk/Auto Add’. It can be made to ignore folders with no video files and recycle bin from the configuration options. If specific folders should be ignored, then they can be from the within the tools. (specify ignore folders)

### **Automated Addition**

TV Rename can look at ‘spare’ files in the ‘download’/Search folders;

* If it cannot find a home for them then
* It tries to find the series on TVDB and asks the user for clarification via a streamlined add dialog.
* Once accepted, TVR automatically adds the show.
* If auto folder creation is on, then the folders get created in the library automatically and the appropriate files copied in.

### Further Information <a href="#further-information" id="further-information"></a>

This function can be turned on using the tick box in [**Options>Preferences>Bulk / Auto Add - Notify when new shows are found**](https://www.tvrename.com/manual/options#the-bulk--auto-add-tab). There are options here to help modify filenames into show names by ignoring certain terms and by ignoring files altogether with specific terms in the filename.
