---
description: Contribute by keeping profiles up-to-date
---

# First Time Maintainer
## Getting Started
Before we dive into editing anything, there are a few things you need to check first. </br>
Don't worry! We've explained everything you need to know below.

***

## Prerequisites

### License Check
Original creators have spent plenty of time publishing the profile, so before you begin to make any changes you need to check the profile's license.

#### Explained
There are two types of license:

| License | Description | 
| --- | ----------- |
| CC BY-NC 4.0 | Modifications Allowed |
| CC BY-NC-ND 4.0 | **NO** Modifications Allowed |

You are looking for `CC BY-NC 4.0` in order to have the green light for modifications.
Instead of searching through files, we've complied a list of available profiles and their respective licenses. See [Here]()

✅ If the profile you wish to update is listed as modifyable, then please continue [here](#modifyable)
❌ If it isn't, then please continue below...

***

### Not Modifyable
If you reached this point, it means that the creator has indicated that they wish to reserve any modifications.

You are now in the position to offer suggestions/improvements or report any bugs via the GSX Hub/Profiles GitHub Page.

To do so, please follow this [link](https://github.com/GSX-Hub/Profiles/issues/new/choose)
If you ask me, you may have dodged a bullet 😉 Profiles can be very tedious at times.

> Completed the form? 

Perfect! </br>
The creator may respond and ask for further details, so please keep an eye out.

*On behalf of the creators and GSX Hub, thank you for offering your support.*

***

### Modifyable
So the profile is listed as modifyable, let's get started!

#### Software
Either (Option 1):

- [GitHub Desktop](https://desktop.github.com/download/) - Install and login with GitHub
- Text Editor E.G. Notepad++

Or (Option 2) **Recommended**:

- Visual Studio Code

#### Clone the Repository

=== ":one: GitHub Desktop"

    1. Head over to the [GSX Hub Profiles GitHub Repo](https://github.com/GSX-Hub/Profiles)
    2. Fork the repository by selecting `Fork` on the top bar
    ![HWMxlo6TzW](https://github.com/user-attachments/assets/c1598236-9fee-4769-a4af-4c146c254ea4)

    3. Clone your fork by selecting `<> Code -> Open with GitHub Desktop`. 
    <figure markdown="span">
      ![Image title](https://github.com/user-attachments/assets/ac81bfd1-2fb1-4a19-b015-7c44eecee6cb)
    </figure>
    !!! note
        Make sure it says `forked from GSX-Hub/Profiles` in the top left-hand corner before cloning it.

    ***
    > GitHub Desktop

    1. Choose a suitable location to clone the repository to. We recommend you choose an easily accessible location such as (Documents).

        ![NVIDIA_Overlay_TQ4KW2cGkE](https://github.com/user-attachments/assets/7ae3ce81-0510-4e0e-85f0-d2a5eee95826)

    2. Select `To contribute to the parent project`

        ![NVIDIA_Overlay_NxFhax8vMi](https://github.com/user-attachments/assets/c5ad042f-43f3-4b46-bee3-955b629b5ef8)

    - [x] Cloned the repository to your PC

=== ":two: Visual Studio Code"

    1. Head over to the [GSX Hub Profiles GitHub Repo](https://github.com/GSX-Hub/Profiles)
    2. Fork the repository by selecting `Fork` on the top bar
    ![HWMxlo6TzW](https://github.com/user-attachments/assets/c1598236-9fee-4769-a4af-4c146c254ea4)

    3. Clone your fork by selecting `<> Code -> Copy Git URL`
    <figure markdown="span">
      ![Image title](https://sharex.hinshaw.cloud/screenshots/2025-02/AS7n6ypEeg.png)
    </figure>
    !!! note
        Make sure it says `forked from GSX-Hub/Profiles` in the top left-hand corner before cloning it.

    ***
    > Visual Studio Code

    4. Open Visual Studio Code and select `Clone Git Repository` then paste the URL into the top bar
    <figure markdown="span">
      ![Image title](https://sharex.hinshaw.cloud/screenshots/2025-02/Bw3UhXwF8Y.png)
    </figure>
    5. Choose a suitable location to clone the repository to
    !!! example
        Something like `Documents/GitHub/` would be sensible

    - [x] Cloned the repository to your PC

***

#### Creating a branch

=== ":one: GitHub Desktop"
    1. Inside of GitHub Desktop, ensure that the 'Current repository' is `Profiles`, the 'Current branch' is `main` and select `New Branch`.
    ![image](https://github.com/user-attachments/assets/47f7f79a-fc73-42bf-97db-430d2700184b)

    2. Name your branch in accordance with the issue number: `issue-12`
    <figure markdown="span">
        ![image](https://sharex.hinshaw.cloud/screenshots/2025-02/GitHubDesktop_aWgILxVmlu.png)
    </figure>
    Now that you have created the branch, we can begin to make the necessary changes.

    - [x] Created a branch

=== ":two: Visual Studio Code"



#### Making the changes
Now that we have made the branch, you can make the changes required.
Using the text editor of your choice, edit the files and return to this section once you are complete.
##### Good Habits
Below are some good habits to get into when editing, some are GitHub related.

| Tip | Description |
| --- | --- |
| Commit Periodically | Ideally you should be committing your changes regularly. For example, if I was to modify a group of stands (Terminal A), before I move to Terminal B stands I will commit the changes made. It allows for natural breaks in development and, if you publish the branch, others can help support and view your progress. |


#### Ready to Upload?
Feel you've forgotten or messed something up? Don't worry - it will be checked before it goes live.

=== ":one: GitHub Desktop"
    1. Open GitHub Desktop and notice the list of changes on the left-hand side. You can go through them and check to see if it has detected all your changes. If anything is missing, double check you have saved the file.

    2. Name your commit. Since this is your first commit of the profile, I highly recommend naming it `Initial Release`. You may add a description should you wish.

    3. Once you have selected `Commit to...` you can then select `Publish Branch` at the top. This will push the branch to GitHub and allow your changes to be compared against the main code.

=== ":two: Visual Studio Code"

    To Complete

##### Creating a Pull Request (PR)
Now that the branch has been published to your GitHub Repo, it's time to make a Pull Request against the existing files.

1. Navigate back to the repository's [main page](https://github.com/GSX-Hub/Profiles). You should see this notification:

![ox6CYKctXY](https://github.com/user-attachments/assets/67eb64a1-7abe-4941-8a0a-1493dde4f3ba)

2. Click `Compare & Pull Request`. Fill out the PR form like the example below:

![fyRlWuymka](https://github.com/user-attachments/assets/7d745862-eba6-4cf9-bef5-5556bacd8967)

!!! tip
    You must follow the PR schema. `[ICAO] Developer | Fixes #[IssueNumber]`
    !!! example
        `[EGNX] Pyreegue | Fixes #12`

When you are happy, submit the PR by clicking `Create Pull Request`.