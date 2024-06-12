learn from chai aur code tutorial

install
 

 1. Git Config
To start using Git, you need to configure it. This command allows you to specify the username and email address that will be used with your commits.

Copy code
# sets up Git with your name
git config --global user.name "<Your-Full-Name>"
# sets up Git with your email
git config --global user.email "<your-email-address>"
2. Git Init
A Git repository must first be created before you can make commits or do anything else with it. We’ll use the git init command to create a new Git repository.

Copy code
$ git init
3. Git Clone
The git clone command produces a local working copy of a remote repository’s source code.

Copy code
$ git clone https://github.com/<repo-url>
4. Git Status
The git status command gives us all the necessary information about the current state of our repository.

Copy code
git status
5. Git Add
The git add command is used to stage changes. It adds the changes in the working directory to the staging area.

Copy code
git add <file1> <file2> … <fileN>
or

Copy code
$ git add .
6. Git Commit
The git commit command saves a log message along with the commit id of the modifications made to the Git repository.

Copy code
$ git commit –m "<Type your commit message here>"
7. Git Push
The git push command pushes the contents of your local repository to the remote repository you’ve added.

Copy code
$ git push
8. Git Branch
The git branch command is used to perform operations on a branch that has been specified.

Copy code
$ git branch <branch-name>
or

Copy code
$ git branch or $ git branch --list
9. Git Checkout
The git checkout command is used to switch to an existing branch or to create and switch to a new one.

Copy code
git checkout <name-of-your-branch>
or

Copy code
git checkout -b <name-of-your-branch>
10. Git Merge
The git merge command integrates your feature branch with all of its commits back to the dev (or master) branch.

Copy code
git checkout dev
git fetch
git merge <branch-name>
11. Git Pull
The git pull command fetches the contents of the remote repository and integrates it into your local repository.

Copy code
$ git pull
12. Git Log
The git log command is used to show all of a repository’s commits.

Copy code
$ git log
13. Git Revert
The git revert command is used to undo the changes that we've made.

Copy code
git revert <commit-id>
14. Git Remote
The git remote command is used to manage the set of repositories that are tracked.

Copy code
git remote add <name> <url>
15. Git Tag
The git tag command is used to create, list, and delete tags.

Copy code
git tag <tag-name>
These are the essential Git commands that every developer should know.




add more useful command for gitbash


How to add more commands to Git Bash? - Super User


superuser
how to add more utilities to git bash for windows, wget, make · GitHub


gist.github
Why can't I use "more" command in Git Bash? [closed] - Stack Overflow


stackoverflow
Git bash: Definition, commands, & getting started - Atlassian


atlassian
Here are some additional useful Git commands for Git Bash:

Reverse a given commit with SHA
bash
Copy code
git revert <sha of commit to revert>
Erase (reset) commits
bash
Copy code
git reset <reference-to-commit>
git reset --soft HEAD^
Git Reset's Flags
The way that Git determines if it erases, stages previously committed changes, or unstages previously committed changes is by the flag that's used. The flags are:

--mixed: take the changes made in commit and move them to the working directory
--soft: the changes moved to the Staging Index
--hard: The changes are completely erased
Backup Branch
bash
Copy code
git branch backup
Push Date to Github Repo
bash
Copy code
git push -u origin master
Configure Git
bash
Copy code
git config --global user.email "<your-email-address>"
git config --global color.ui auto
git config --global merge.conflictstyle diff3
git config --list
Git & Code Editor
bash
Copy code
git config --global core.editor "atom --wait"  # for Atom Editor
git config --global core.editor "C:Program Files/SublimeText2/sublime_text.exe' -n -w"  # for Sublime Text
git config --global core.editor "code --wait"  # for VSCode
Repository Commands
bash
Copy code
git init  # create a new repository
git clone <url>  # copy an existing repository
git status  # check the status of a repository
Review Repo History
bash
Copy code
git log  # displays information about the existing commits
git log --oneline  # shows the first 6 letters of SHA and the commit message
Branching
bash
Copy code
git branch  # list all branch names in the repository
git branch <branchname>  # create a new branch
git branch <branchname> <sha-id of existing branch>  # create a new branch from an existing commit
git branch -d <branchname>  # delete a branch
git checkout <branchname>  # change the branch
Merging
bash
Copy code
git merge <name-of-branch-to-merge-in>  # combine the differences of different branches
Tagging
bash
Copy code
git tag -a v1.0  # add a tag to a specific commit
git tag -d v1.0  # delete a tag
git tag  # show all existing tags
Other Commands
bash
Copy code
git rm --cached <filename>  # remove files from the staging index
git commit  # commit files
git commit -m "Initial commit"  # commit with a message
git diff  # displays the difference between two versions of commits
I hope these additional commands are helpful!


