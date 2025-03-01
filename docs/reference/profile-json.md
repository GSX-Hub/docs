---
description: Profile.json Schema
hide: toc
---


``` json title="profile.json"
{
    "ProfileICAO": "EGPH", // (1)!
    "Scenery": "Pyreegue (v2)", // (2)!
    "Creator": "Hinshee", // (3)!
    "Version": 1.1, // (4)!
    "Configurations": [
        {
            "ConfigName": "GSX", // (5)!
            "Files": [ // (6)!
                {
                    "FileName": "egph-pyreegue-hinshee.ini"
                },
                {
                    "FileName": "egph-pyreegue-hinshee.py" // (7)!
                }
            ]
        }
    ],
    "Changelog": [
		{
            "Version": 1.1,
            "ChangesURL": "https://github.com/Hinshee/GSX-Profiles/pull/13", // (8)!
			"Date": "2024-07-27" // (9)!
        },
        {
            "Version": 1,
            "ChangesURL": "",
		    "ChangesMd": "* Initial release", // (10)!
			"Date": "2024-07-19"
        }
    ]
}
```

1.  The 4 Letter ICAO code for the profile. Uppercase is preferred.
2.  Scenery Developer
3.  Original Creator(s)
4.  Current version profile number
5.  Name of the configuration. Example: `GSX` and `ASVDGS`
6.  List of files that are required for this configuration
7.  The exact name of the required file. `Case-Sensitive. Must match`
8.  `Optional` URL for link to changes.
9.  Date of Update. Format: YYYY-MM-DD
10. Markdown content for changelog

#### Main
| Entry | Description | Parameters |
| --- | ----------- | ----------- | 
| ProfileICAO | The 4 Letter ICAO code for the profile. | Uppercase Preferred |
| Scenery | Scenery Developer | -- |
| Creator | Original Creator(s) | -- |
| Version | Current version profile number | -- |

#### Configurations
Important section if you have multiple configurations (i.e. multiple .ini or .py files)

| Entry | Description | Parameters |
| --- | ----------- | ----------- |
| ConfigName | Name of the configuration | Uppercase Preferred |
| Files | List of files that are required for the configuration | -- |
| FileName | The exact name of the required file | Case-Sensitive. Must match |

#### Changelog
| Entry | Description | Parameters |
| --- | ----------- | ----------- | 
| Version | -- | -- |
| ChangesURL | URL for link to changes | Can be empty |
| ChangesMD | Markdown content for changelog | -- |
| Date | Date of Update | Format: YYYY-MM-DD |