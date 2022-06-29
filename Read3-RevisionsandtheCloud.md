Git is a VCS (version control system. It keeps track of changes
It  allows others to work on the same document simlultanesously. 
It gives the option to review and commit changes

Git makes collaboration possible.

Think of Git as making snapshots in time of a project. 

A repository is simply a folder or directory that is being tracked with Git.

Commits represent each successive version of a file or files. They are the equivalent of a “save as”
Each successive version creates a new snapshop on the timeline of the project.

Commits in Github
Each commit has a label that points to it. The “HEAD” label is the label meaning “This is the most current version”. Best practice: One should assign messages to commits. 
Best practice: Keep the commit message to 50 characters or less to avoid having it truncated. 

Git vs. Github
Git = Version Control
Github = online storage

A repository is a collection of files that you’ve told Git to pay attention to. They can live in Github, or on your computer on Git. Files in a repository should be related to one another. If they are not related, they should be stored in a separate repository. Often times there will be a Front End and Back End repository.

Create new repository
Select owner
Name the repository

Making the repository into a Website using the github templates.
Setting → Pages → Branch=Main → Root -> Save (generates a url) → select a theme → copy the url and put it in the “about” section, so that it will be easily accessible.


How to bring a repository down to your computer (cloning)r:
Go to the repository’s home page
Click the Green Code button
Make sure HTTPs is selected
Select all of the text (link)
Open Terminal and create a folder for the files to live in, (Projects) (Courses)
Once you are in the final folder where it will be stored, use the command ‘git clone’ and then paste the link.
(Make sure that the folder where you wish to work (on VSCode) is being tracked by git ‘git:(main)
Use ‘code .’



Commands:

To send changes back to Github: SACP 
S = Status: git status (shows the changes) Tells you the branch you’re on. Shows files that are not yet tracked by git.

A=collecting what files you want to save in this ‘snapshot’

A=git add ‘filename1’ ‘filename2’
git add . (will add all of the files)

Git restore --staged ‘filename’ (removes that file from being staged for commitment)

C=commit
git commit -m “message” (use double quotes)

(the -m “ “ is a message tag.)

P= Push

git push origin main

https://github.com/JoseGonzalez1394/Marvel#:~:text=josegonzalez1394.github.io/marvel/

Gituation i.e. a Git Conflict:

Best practice: once a repository is cloned from github to one’s computer (local) then it will be best to work in the code editor (VS Code).

Best practice: When you accomplish a feature, ACP!

Clone…
Make changes in one file - then ACP
Make changes in another file - then ACP

git help

git log : shows a log of all of the different commits that have been done.
