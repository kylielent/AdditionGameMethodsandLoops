#Project 2
# AdditionGameMethodsandLoops 

##Introduction
This is code that uses a for loop, a custom method call and an array on our earlier addition game.
This process is used in eclipse and through github.

##Code
```java
```

##Console
```java
```

##Command Prompt
```
This is my flashdrive
C:\Users\LAB>E:

I type dir to see the directory of my files
E:\>dir


 Directory of E:\

10/13/2015  07:36 PM    <DIR>          Workspace
02/06/2015  07:43 AM    <DIR>          College Assignments
02/06/2015  07:43 AM    <DIR>          Senior Pictures
10/05/2015  06:50 PM    <DIR>          IF FOUND, OPEN ME
11/09/2015  09:41 AM    <DIR>          Methods
11/09/2015  09:41 AM    <DIR>          MandLoops
11/19/2015  06:08 PM    <DIR>          Arrays
11/20/2015  09:31 AM    <DIR>          AdditionGameMethodsandLoops
               0 File(s)              0 bytes
               8 Dir(s)   3,521,880,064 bytes free

I type cd to choose what folder I want to be in
E:\>cd AdditionGameMethodsandLoops

I type dir again to see the directory inside that folder
E:\AdditionGameMethodsandLoops>dir

 Directory of E:\AdditionGameMethodsandLoops

11/20/2015  09:31 AM    <DIR>          .
11/20/2015  09:31 AM    <DIR>          ..
11/20/2015  09:31 AM    <DIR>          .metadata
11/20/2015  09:31 AM    <DIR>          AdditionGame
               0 File(s)              0 bytes
               4 Dir(s)   3,521,880,064 bytes free

E:\AdditionGameMethodsandLoops>cd AdditionGame

E:\AdditionGameMethodsandLoops\AdditionGame>dir

 Directory of E:\AdditionGameMethodsandLoops\AdditionGame

11/20/2015  09:31 AM    <DIR>          .
11/20/2015  09:31 AM    <DIR>          ..
11/20/2015  09:31 AM               388 .project
11/20/2015  09:31 AM    <DIR>          src
11/20/2015  09:31 AM    <DIR>          bin
11/20/2015  09:31 AM               232 .classpath
               2 File(s)            620 bytes
               4 Dir(s)   3,521,880,064 bytes free

Here I create the read me file for my repository
E:\AdditionGameMethodsandLoops\AdditionGame>echo # AdditionGameMethodsandLoops >
> README.md

I type git init to intialize the repository into my flashdrive
E:\AdditionGameMethodsandLoops\AdditionGame>git init
Initialized empty Git repository in E:/AdditionGameMethodsandLoops/AdditionGame/
.git/

Here I add the readme
E:\AdditionGameMethodsandLoops\AdditionGame>git add README.md

Here I commit what I have just done
E:\AdditionGameMethodsandLoops\AdditionGame>git commit -m "first commit"

*** Please tell me who you are.

Run

  git config --global user.email "you@example.com"
  git config --global user.name "Your Name"

to set your account's default identity.
Omit --global to set the identity only in this repository.

fatal: unable to auto-detect email address (got 'LAB@STF126H-PC.(none)')

Here I configure my username and email because I forgot to earlier
E:\AdditionGameMethodsandLoops\AdditionGame>git config user.name "kylielent"

E:\AdditionGameMethodsandLoops\AdditionGame>git config user.email "lentk@student
.swosu.edu"

Then i re-commit what I did earlier
E:\AdditionGameMethodsandLoops\AdditionGame>git commit -m "first commit"
[master (root-commit) 722e994] first commit
 1 file changed, 1 insertion(+)
 create mode 100644 README.md

Here I add to the origin
E:\AdditionGameMethodsandLoops\AdditionGame>git remote add origin https://github
.com/kylielent/AdditionGameMethodsandLoops.git

Here I push to the origin master
E:\AdditionGameMethodsandLoops\AdditionGame>git push -u origin master

Here I login to github with my username and password
Username for 'https://github.com': kylielent
Password for 'https://kylielent@github.com':
Counting objects: 3, done.
Writing objects: 100% (3/3), 245 bytes | 0 bytes/s, done.
Total 3 (delta 0), reused 0 (delta 0)
To https://github.com/kylielent/AdditionGameMethodsandLoops.git
 * [new branch]      master -> master
Branch master set up to track remote branch master from origin.


Here I add what I have been working on
E:\AdditionGameMethodsandLoops\AdditionGame>git add .

Here I commit the changes
E:\AdditionGameMethodsandLoops\AdditionGame>git commit -m "code is working."
[master 1aa313f] code is working.
 4 files changed, 95 insertions(+)
 create mode 100644 .classpath
 create mode 100644 .project
 create mode 100644 bin/AdditonGameMethodsandLoops.class
 create mode 100644 src/AdditonGameMethodsandLoops.java

Here I push to the master branch
E:\AdditionGameMethodsandLoops\AdditionGame>git push
warning: push.default is unset; its implicit value has changed in
Git 2.0 from 'matching' to 'simple'. To squelch this message
and maintain the traditional behavior, use:

  git config --global push.default matching

To squelch this message and adopt the new behavior now, use:

  git config --global push.default simple

When push.default is set to 'matching', git will push local branches
to the remote branches that already exist with the same name.

Since Git 2.0, Git defaults to the more conservative 'simple'
behavior, which only pushes the current branch to the corresponding
remote branch that 'git pull' uses to update the current branch.

See 'git help config' and search for 'push.default' for further information.
(the 'simple' mode was introduced in Git 1.7.11. Use the similar mode
'current' instead of 'simple' if you sometimes use older versions of Git)

Here I login again
Username for 'https://github.com': kylielent
Password for 'https://kylielent@github.com':
Counting objects: 8, done.
Delta compression using up to 4 threads.
Compressing objects: 100% (8/8), done.
Writing objects: 100% (8/8), 2.79 KiB | 0 bytes/s, done.
Total 8 (delta 0), reused 0 (delta 0)
To https://github.com/kylielent/AdditionGameMethodsandLoops.git
   722e994..1aa313f  master -> master

E:\AdditionGameMethodsandLoops\AdditionGame>
We are done!
```

##Summary
The purpose of this project was to take what we have done with for loops, methods and arrays and apply it to the additon game. Which is an easy assignment that we pull for a lot of our projects to experiment on more.


