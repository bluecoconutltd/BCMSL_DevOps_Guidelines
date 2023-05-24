# a. Developer Notes

## a.1 Automatic Signed Project Releases

### **Pushing a Signed Project Release to GitHub**

The following arguments sets the tag name, signs the tag using GPG, verifies the signed tag, and then runs release-it. You can customize the configurations to fit your needs. Before running this script, make sure that you have GPG installed and configured on your system. You will also need to have a GPG key pair and tell Git about your signing key.  

* **a.1.1** - To sign your tags automatically with GPG and release-it before pushing them to GitHub, ensure the following arguments that signs your tags are set properly ***`"git.tagArgs":["-s"]`*** to ensure the tags are signed in Git, ***`"git.push": true`***, ***`"git.pushArgs": ["--follow-tags"]`***:  

!!! info "List of All Default Release-it Arguments"

    * These can be added (as necessary) to the release-it settings in the :material-file:`package.json` located in the root of your project directory.
    ```json title="package.json"
        {
      "hooks": {},
      "git": {
        "changelog": "git log --pretty=format:\"* %s (%h)\" ${from}...${to}",
        "requireCleanWorkingDir": true,
        "requireBranch": false,
        "requireUpstream": true,
        "requireCommits": false,
        "requireCommitsFail": true,
        "commitsPath": "",
        "addUntrackedFiles": false,
        "commit": true,
        "commitMessage": "Release ${version}",
        "commitArgs": [],
        "tag": true,
        "tagExclude": null,
        "tagName": null,
        "tagMatch": null,
        "tagAnnotation": "Release ${version}",
        "tagArgs": [],
        "push": true,
        "pushArgs": ["--follow-tags"],
        "pushRepo": ""
      },
      "npm": {
        "publish": true,
        "publishPath": ".",
        "publishArgs": [],
        "tag": null,
        "otp": null,
        "ignoreVersion": false,
        "allowSameVersion": false,
        "versionArgs": [],
        "skipChecks": false,
        "timeout": 10
      },
      "github": {
        "release": false,
        "releaseName": "Release v${version}",
        "releaseNotes": null,
        "autoGenerate": false,
        "preRelease": false,
        "draft": false,
        "tokenRef": "GITHUB_TOKEN",
        "assets": null,
        "host": null,
        "timeout": 0,
        "proxy": null,
        "skipChecks": false,
        "web": false,
        "comments": {
          "submit": false,
          "issue": ":rocket: _This issue has been resolved in v${version}. See [${releaseName}](${releaseUrl}) for release notes._",
          "pr": ":rocket: _This pull request is included in v${version}. See [${releaseName}](${releaseUrl}) for release notes._"
        }
      },
      "gitlab": {
        "release": false,
        "releaseName": "Release ${version}",
        "releaseNotes": null,
        "milestones": [],
        "tokenRef": "GITLAB_TOKEN",
        "tokenHeader": "Private-Token",
        "certificateAuthorityFile": null,
        "assets": null,
        "origin": null,
        "skipChecks": false
      }
    }


    ```
    * Add Developer Note Here! >>  :
    ```bash
    << add code here >>
    ```
    * Add Developer Note Here! >>  :
    ```bash
    << add code here >>
    ```
    << Add Developer Note Here! >>  : 
    ```bash
    << add code here >>
    ```

* **a.1.2** - << Add Developer Note Here! >>  

!!! info inline end "Note: CLI Terminal Usage"

    These images are basic examples. Both **:simple-windowsterminal: CMD** or **:material-powershell: PowerShell** Terminals would produce the same outputs or trigger the necessary terminal when running commands. Unless explicitly advised in certain instances, the developer would be required to manually switch to a specific CLI to run some commands. Example: Using :material-git: Git Bash for Unix-like Commands.
  
***

* **a.1.3** - << Add Developer Note Here! >>

* **a.3.4** - << Add Developer Note Here! >>  

***
!!! note-license inline "License Notice"
  
    [Blue Coconut Multimedia Solutions Limited](https://bluecoconut.ltd)  
    52A Eccles Road, Grand Lagoon,  
    Mayaro, Trinidad and Tobago, W.I.  
    <info@bluecoconut.ltd>  
    --------------------------
    [MIT License (2023)](license.md)  
    ![BCMSL](assets/img/BCMSL LOGO DARK.svg#only-light){ width="50px" } ![BCMSL](assets/img/BCMSL LOGO LIGHT.svg#only-dark){ width="50px" }
