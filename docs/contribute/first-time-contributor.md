---
description: For GSX Profile Owners
---

# First Time Contributor
## Getting Started
!!! tip
    Before reading on, please ensure you have read and understood the [licensing agreement](licensing.md) that GSXHub operates. </br>
    Should you have any questions regarding this, please contact us via the [GSX Community Discord](https://discord.gg/ubCkJQS6Mj).

### Prerequisites
In order to make contributing straight-forward, we've compiled a list of prerequisites:

- [GitHub Desktop](https://desktop.github.com/download/) - Install and login with GitHub
- A completed GSX Profile
- 15 Minutes of your time 😉

***

## Clone the Repository
1. Head over to the [GSX Hub Profiles GitHub Repo](https://github.com/GSX-Hub/Profiles)
2. Fork the repository by selecting `Fork` on the top bar
![HWMxlo6TzW](https://github.com/user-attachments/assets/c1598236-9fee-4769-a4af-4c146c254ea4)

3. Clone your fork by selecting `<> Code -> Open with GitHub Desktop`. 
<figure markdown="span">
  ![Image title](https://github.com/user-attachments/assets/ac81bfd1-2fb1-4a19-b015-7c44eecee6cb)
</figure>
!!! note
    Make sure it says `forked from GSX-Hub/Profiles` in the top left-hand corner before cloning it.

- [x] Cloned the repository to your PC
***

## GitHub Desktop
1. Choose a suitable location to clone the repository to. We recommend you choose an easily accessible location such as (Documents).

![NVIDIA_Overlay_TQ4KW2cGkE](https://github.com/user-attachments/assets/7ae3ce81-0510-4e0e-85f0-d2a5eee95826)

2. Select `To contribute to the parent project`

![NVIDIA_Overlay_NxFhax8vMi](https://github.com/user-attachments/assets/c5ad042f-43f3-4b46-bee3-955b629b5ef8)

- [x] Downloaded and setup the repository
***

### Creating a branch

1. Inside of GitHub Desktop, ensure that the 'Current repository' is `Profiles`, the 'Current branch' is `main` and select `New Branch`.
![image](https://github.com/user-attachments/assets/47f7f79a-fc73-42bf-97db-430d2700184b)

2. (Optional) Name your branch in accordance with the profile you intend to upload.
!!! hint
    You could use a schema such as: `ICAO-Developer-Creator`

![image](https://github.com/user-attachments/assets/66df0cd7-17c2-4d45-a843-3d280ea510b1)

Now that you have created the branch, we can start to add the profile to the repository.

- [x] Created a branch
***

### Preparing the folder

Now that we have cloned the repository we can now create the folder which our profile will be in.

1. Navigate to the folder which you selected back in [Clone the Repository](#clone-the-repository) step. In my case, this will be `Documents\GitHub\Profiles`.

You should be presented with the repository files such as `availprofiles.json` and the `Airports` folder.

![explorer_irBTOL4F8c](https://github.com/user-attachments/assets/8beacd80-81a4-422f-8947-1cacd055ef7a)

2. Navigate to the `Template` folder and copy the folder named `ICAO (Developer)` to the `Airports` folder. Contained within `ICAO (Developer)` is all the necessary files required to host on GSXHub.

3. Rename the `ICAO (Developer)` you've just copied to `Airports` using the standard format. 
!!! example "Examples"
    ✅ `EGNX (Pyreegue)`, `EDDM (SimWings)` </br>
    ❌ `EGPH (Hinshee)`, `EIDW (SimonTricks)` - These are the creators' names, not the scenery developer

![explorer_vstiDpFY33](https://github.com/user-attachments/assets/c4a328ed-55b2-49ad-af64-3f963847e0b0)

For this demonstration, we'll use the example `EFOU (M'M Simulations)`.

Your folder should look like this:

![explorer_QvUHv5g4Cm](https://github.com/user-attachments/assets/dca01d34-b29c-438c-88ed-c6d437ea9bb4)

- [x] Preparing the folder

***

### Uploading Files

With the folder setup, you can now add your profile files.

![9PHBkEZmpm](https://github.com/user-attachments/assets/d81f3902-70fe-4b41-beec-f547ea2e4309)

1. Remove the placeholder file `Install Profiles Here.txt`.
2. Add your `.ini` and `.py` files.

3. You must add the following line to all your files indicating the file's current version: `version = X.X`

!!! example
    ![notepad++_6i0nWdMtet](https://github.com/user-attachments/assets/3a26b3a8-d0fe-4ea2-99e6-bd5868996554)
    Note the highlighted 'version' lines that have been added.
***

### Modifying `profile.json`

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

The included file is filled out to help.
Here is every entry explained and what is required:

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

✅ Here is the finished demonstration example:

``` json title="profile.json"
{
    "ProfileICAO": "EFOU",
    "Scenery": "M'M Simulations",
    "Creator": "Hinshee",
    "Version": 1,
    "Configurations": [
        {
            "ConfigName": "GSX",
            "Files": [
                {
                    "FileName": "efou-mmsimulations-hinshee.ini"
                },
                {
                    "FileName": "efou-mmsimulations-hinshee.py"
                }
            ]
        }
    ],
    "Changelog": [
		{
            "Version": 1,
            "ChangesURL": "",
			"Date": "2024-12-24"
        }
    ]
}
```

#### Multiple Configurations

A good example for multiple configurations is [EDDM (SimonTricks)](https://github.com/GSX-Hub/Profiles/blob/main/Airports/EDDM%20(Simwings)/profile.json)

***

### Modifying `Information.md`

![TftGVtUYvQ](https://github.com/user-attachments/assets/b7ba3e99-4e2c-49df-809b-5fe4aa9b02bb)

`Information.md` is a markdown file that will display within the application.
Please refer to this [file](https://github.com/GSX-Hub/Profiles/blob/main/.github/Compatible_Markdown.md) to see what markdown features are supported.

#### Adding your license

As explained within the [licensing agreement](licensing.md) you must choose which license you wish your profile to fall under. 

You must add one of the following lines to the top of your Markdown file:

* `<!--- Licensed Under: CC BY-NC 4.0 --->` = Attribution required; noncommercial use only; modifications allowed.
* `<!--- Licensed Under: CC BY-NC-ND 4.0 --->` = Attribution required; noncommercial use only; no modifications or derivative works allowed.

Leave the `<!---` and `--->` as this will prevent it being shown via the App. </br>
The comment will help GitHub Actions determine if it should allow modifications if they are requested.

!!! example
    ``` md title="Information.md" hl_lines="1"
        <!--- Licensed Under: CC BY-NC 4.0 --->

        Available from these retailers: 
        - Contrail.shop: [Affiliate Link](https://contrail.shop/xoiedo) / [Non-Affiliate Link](https://contrail.shop/products/mm-simulations-efou-oulu-airport-msfs)
        ...

        ### Features:
        - Custom Vehicle Positioning
        - Walk-in gates (Stands 13B, 12A, 11, 10, 9)
        - Custom Pushbacks
        - Accurate Ground Handling Agents
    ```
***

## Ready to Upload?
Feel you've forgotten or messed something up? Don't worry - it will be checked before it goes live.

1. Open GitHub Desktop and notice the list of changes on the left-hand side. You can go through them and check to see if it has detected all your changes. If anything is missing, double check you have saved the file.

2. Name your commit. Since this is your first commit of the profile, I highly recommend naming it `Initial Release`. You may add a description should you wish.

3. Once you have selected `Commit to...` you can then select `Publish Branch` at the top. This will push the branch to GitHub and allow your changes to be compared against the main code.

![GF3exCzXPz](https://github.com/user-attachments/assets/19ef48d2-6ce4-46a0-bdbd-94c8d3bcd61a)

Once published, navigate back to the repository's [main page](https://github.com/GSX-Hub/Profiles). You should see this notification:

![ox6CYKctXY](https://github.com/user-attachments/assets/67eb64a1-7abe-4941-8a0a-1493dde4f3ba)

4. Click `Compare & Pull Request`. Fill out the PR form like the example below:

![fyRlWuymka](https://github.com/user-attachments/assets/7d745862-eba6-4cf9-bef5-5556bacd8967)

!!! tip
    Change the title of the PR to something sensible. You could follow this schema: `[ICAO] Developer | Initial Release`
    !!! example
        `[EFOU] M'M Simulations | Initial Release`

When you are happy, submit the PR by clicking `Create Pull Request`.

- [x] Submit your profile </br>
🎉Whoop! You've submitted your first profile to GSXHub 🎉

***

## Checks
Now you've successfully submitted your first Pull Request with your profile, it requires _at least_ one senior moderator to check and ensure everything complies. 
</br></br>
They are notified of a new request so there's no need to ping via Discord. If there are any problems, they will contact you within the PR. This can take up to 48 hours depending on their availability.

***

## Questions?
Struggling with something? Please contact us via the [GSX Community Discord](https://discord.gg/ubCkJQS6Mj)