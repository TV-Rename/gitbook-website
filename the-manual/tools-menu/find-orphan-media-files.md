---
description: Finds video files in the library that might not need to be there
---

# Find Orphan Media Files

This tool scans through the TV Library to find files that might not need to be in the library.

![](<../../.gitbook/assets/image (4).png>)

It identifies 4 types of file:

| Type                                     | Description                                                                                                                                                                                               |
| ---------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| File does not match a Filename Processor | The file is in the library, but the filename does not match any of the filename processors. Therefore TV Rename cannot work out which season / episode it is meant to be for.                             |
| File is in the wrong series folder       | The file seems to relate to a specified season, but it is stored in another season's folder.                                                                                                              |
| Season not found                         | The file matches a filename processor, but the filename processor has looked at the filename and considers it to be part of a season that does not exist (according to the source provider for that show) |
| Episode not found                        | The file matches a filename processor, but the filename processor has looked at the filename and considers it to be am episode that does not exist (according to the source provider for that show)       |

The information is presented only for information. Right clicking gives some options to review:

1. The folder that contains the file
2. The Episode Guide within TV Rename
3. The Source Provider's view of the show

If you get many files that have been mapped to the incorrect season/episode then you may need to review the Filename Processors to adjust them to interpret files correctly.

{% content-ref url="../options-menu/filename-processors.md" %}
[filename-processors.md](../options-menu/filename-processors.md)
{% endcontent-ref %}
