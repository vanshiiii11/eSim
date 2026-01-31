## Contribution
If you want to add any enhancement feature or have found any bug and want to work on it, please open a new issue regarding that and put a message "I would like to work on it." And make sure every pull request should reference to an issue.

#### Points on how to make pull request
* You need to fork this repository to your account.  

* Clone it using ``` git clone https://github.com/FOSSEE/eSim.git ```

* Always create a new branch before making any changes. You can create new branch using ```git branch <branch-name> ```

* Checkout into your new branch using ```git checkout <branch-name>```

* Make changes to code and once you are done use ```git add <path to file changed or added>```. Now commit  changes with proper message using ```git commit -m "Your message"```.

* After commiting your changes push your changes to your forked repository using ```git push origin <branch-name>```
Finally create a pull request from github.
There should be only one commit per pull request.


* Please follow below guidelines for your commit message :
  * Commit message should be like : Fixes issue #[issue_number] - one line message of work you did.
  * After commit message, there should be a commit body where you can mention what you did in short or in detail.

Please follow above method to file pull requests.
---

## 🧪 Contribution Notes (Ubuntu 25.04)

While setting up this project on **Ubuntu 25.04 (VM)**, the following issues were encountered and resolved:

### SSH Authentication Issue
- Initial `git push` attempts failed with:
  `Permission denied (publickey)`
- Root cause: SSH key not added to GitHub account

### Resolution
- Generated SSH key using:
  `ssh-keygen -t ed25519`
- Added `id_ed25519.pub` to GitHub → Settings → SSH and GPG keys
- Started ssh-agent and added key:
  `eval "$(ssh-agent -s)"`
  `ssh-add ~/.ssh/id_ed25519`
- Verified connection:
  `ssh -T git@github.com`

Push succeeded after completing these steps.

Tested and documented by **Vanshika Motwani (2026)**.
