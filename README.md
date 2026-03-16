# learnable_one
Backend git task on learnable


### Explain version control.
Version control is a workspace that is used to track changes made to a document over time, it shows who made the change and when. It can be used to store or keep track of multiple version of a document/product if possible.


### Explain difference between git and github
The major difference is that git, using git syntax is used to manage documents remotely, so it's a version control tool for local files where github is web-based and allows people to collaborate


### List 3 other github alternatives
- GitLab
- Bitbucket
- Codeberg


### Explain the difference between git fetch and git pull,
Git fetch and git pull are both Git commands used to retrieve update information from a remote repository.
The thing is that:
- Git fetch downloads the changes from the remote repository to the local repository but does not make any changes to the current working directory.  Since the changes are not merged into the local branch, you can check the changes from the remote repository without interrupting your current work.
-  Git pull retrieves the latest changes from the remote repository like git fetch, but it also automatically merges those changes into the current branch. In contrast to git fetch, git pull directly applies the changes from the remote repository to the local working directory.



### Explain in simple terms git rebase and the command for it

Git rebase is a command used to integrate changes from one Git branch into another by moving, or "replaying," a series of commits on top of a new base commit. Rebasing is like taking your changes and placing them on top of the latest version of the main branch or the "source of truth" branch, making it look as if you started your work from that current point or branch, this rewrites the commit history entirely

The command for rebasing: 

- Fetch from the origin
 ```
 git fetch origin 
 ```

- Move to the branch you want to rebase from the origin
 ```
 git checkout feature 
 ```

- Run the rebase command
 ```
git rebase origin/main
 ```



### Explain in simple terms git cherry-pick and the command for it 
Git cherry-pick is used to copy specific changes from an existing branch into your current branch, the command allows you to take a specific commit from one branch and apply it onto another branch, so it allows you to take specific code from a commit that is useful instead of merging an entire branch that is possibly problematic to the project.

the command:
- First you get the log and it shows you the list commit hashes and your target hash
 ```
 git log 
 ```

- Switch to your target branch you want to apply the commit that you want to cherry-pick
 ```
 git checkout main
 ```

- Apply the commit 
 ```
 git cherry-pick <your chosen commit hash>
 ```


