1.Create a directory named git-basic-exercises

recruit@recruit-Mecer-X102:~$ mkdir git-basic-exercises
recruit@recruit-Mecer-X102:~$ ls
 cd             git-basic-exercises    recruits.md
 CHANGELOG.md  'GIT Basics Exercise'   simo
 cohort.md      Music                  Templates
 Cohort.md      my_files               Umuzi.md
 Desktop        mymy_bio.md            Videos
 Documents      Pictures               workspace
 Downloads      Public                 workspase
 exersice.md    README.md

2.cd into your new directory

recruit@recruit-Mecer-X102:~$ cd git-basic-exercises
recruit@recruit-Mecer-X102:~/git-basic-exercises$ 

3.look at what’s inside using ls -a. It should be empty

recruit@recruit-Mecer-X102:~/git-basic-exercises$ ls -a
.  ..

4.initialize your git repo using git init. Then check ls -a again. Can you spot the difference?

recruit@recruit-Mecer-X102:~/git-basic-exercises$ git init
Initialized empty Git repository in /home/recruit/git-basic-exercises/.git/
recruit@recruit-Mecer-X102:~/git-basic-exercises$ ls -a
.  ..  .git

* yes I see the difference of .  ..  .git.


5.check the status of your repo by typing git status

recruit@recruit-Mecer-X102:~/git-basic-exercises$ git statusOn branch master

No commits yet

nothing to commit (create/copy files and use "git add" to track)

6.type in touch README.md. This creates a new blank file. Then check ls -a and git status again.

recruit@recruit-Mecer-X102:~$ touch README.md
recruit@recruit-Mecer-X102:~$ ls
 cd             Documents              Music         README.md     Videos
 CHANGELOG.md   Downloads              my_files      recruits.md   workspace
 cohort.md      exersice.md            mymy_bio.md   simo          workspase
 Cohort.md      git-basic-exercises    Pictures      Templates
 Desktop       'GIT Basics Exercise'   Public        Umuzi.md
recruit@recruit-Mecer-X102:~$ ls -a
 .                    'GIT Basics Exercise'   README.md
 ..                    .gnupg                 recruits.md
 .bash_history         .gtkrc-2.0             simo
 .bash_logout          .gtkrc-xfce            .sudo_as_admin_successful
 .bashrc               .ICEauthority          Templates
 .cache                .icons                 .themes
 cd                    .linuxmint             .thunderbird
 CHANGELOG.md          .local                 Umuzi.md
 cohort.md             .mozilla               Videos
 Cohort.md             Music                  .vscode
 .config               my_files               .wget-hsts
 Desktop               mymy_bio.md            workspace
 .dmrc                 .node_repl_history     workspase
 Documents             Pictures               .Xauthority
 Downloads             .pki                   .xsession-errors
 exersice.md           .profile               .xsession-errors.old
 git-basic-exercises   Public
recruit@recruit-Mecer-X102:~$ git status
fatal: not a git repository (or any of the parent directories): .git

7.type in git log. The output should make sense to you

recruit@recruit-Mecer-X102:~$ git log
fatal: not a git repository (or any of the parent directories): .git

8.Now add your readme file to your git staging area. Hint: use the git add command

recruit@recruit-Mecer-X102:~$ git add
fatal: not a git repository (or any of the parent directories): .git

9.Then check your git status again. Can you see the difference?

recruit@recruit-Mecer-X102:~$ git status
fatal: not a git repository (or any of the parent directories): .git

10.Try to unstage your file and check your git status again


11.Ok, now for your first commit: Make sure your readme file is staged then type in git commit -m "initial commit" Your output should be something like this: [master (root-commit) 2103b64] initial commit 1 file changed, 0 insertions(+), 0 deletions(-) create mode 100644 README.m

recruit@recruit-Mecer-X102:~/git-basic-exercises$ echo "# git-basic-exercises" >> README.md
recruit@recruit-Mecer-X102:~/git-basic-exercises$ git init
Reinitialized existing Git repository in /home/recruit/git-basic-exercises/.git/
recruit@recruit-Mecer-X102:~/git-basic-exercises$ git add README.md
recruit@recruit-Mecer-X102:~/git-basic-exercises$ git commit -m "first commit"
[master 7280180] first commit
 1 file changed, 1 insertion(+)
recruit@recruit-Mecer-X102:~/git-basic-exercises$ git remote add origin https://github.com/SimonZikhali/git-basic-exercises.git
recruit@recruit-Mecer-X102:~/git-basic-exercises$ git push -u origin master
Username for 'https://github.com': SimonZikhali
Password for 'https://SimonZikhali@github.com': 
Counting objects: 6, done.
Delta compression using up to 2 threads.
Compressing objects: 100% (2/2), done.
Writing objects: 100% (6/6), 455 bytes | 455.00 KiB/s, done.
Total 6 (delta 0), reused 0 (delta 0)
To https://github.com/SimonZikhali/git-basic-exercises.git
 * [new branch]      master -> master
Branch 'master' set up to track remote branch 'master' from 'origin'.


MORE COMMITS

1,2,3,4 and5. type in nano README.md. This will open up a text editor. Type in some stuff and then press ctrl x to exit. Then y then enter. This will save your changes type in cat README.md. This will print your file to the console
take a look at the git stats again and make sure you understand it
commit your changes to your repo. Your commit should have the message "second commit"
make some more changes to your readme and make a "third commit"

recruit@recruit-Mecer-X102:~$ nano README.md
recruit@recruit-Mecer-X102:~$ cat README.md
morning
recruit@recruit-Mecer-X102:~$ git stats
git: 'stats' is not a git command. See 'git --help'.

The most similar command is
	status
recruit@recruit-Mecer-X102:~$ cd dir "second commit"
bash: cd: too many arguments
recruit@recruit-Mecer-X102:~$ cd "third commit"
bash: cd: third commit: No such file or directory
recruit@recruit-Mecer-X102:~$ cd dir "third commit"
bash: cd: too many argument

CHECK THIS OUT# git-basic-exercises
# git-basic-exercises
