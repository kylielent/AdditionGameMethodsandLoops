#Project 2
# AdditionGameMethodsandLoops 

##Introduction
This is code that uses a for loop, a custom method call and an array on our earlier addition game.
This process is used in eclipse and through github.

##Code
```java
import java.util.Scanner;
public class AdditonGameMethodsandLoops {
public static void main(String[] args) {
						
		//Call the addition game method.
		AdditonGameMethod();}
					
		public static void AdditonGameMethod() {
		int[] gameVariables = new int[4];
		gameVariables[0] = 5; //This is hardness
		gameVariables[1] = 2; //This is hardness step
		gameVariables[2] = 0; //This is the score
		gameVariables[3] = 0; // 1 for true, 0 for false
						
		// Set up my for loop 
		int numberOfRounds = 4;
			for(int NumberoftheRound = 1; 
				NumberoftheRound <= numberOfRounds;  
				NumberoftheRound = NumberoftheRound + 1){
		System.out.print("Round " + NumberoftheRound + " of " + numberOfRounds + ". ");
		gameVariables = getAndCheckStudentAnswer(gameVariables);
			if(gameVariables[3] == 1){
				System.out.print("Your score was " + gameVariables[2] + " and is now ");
				gameVariables[2] = gameVariables[2] + gameVariables[0];
				System.out.print(gameVariables[2] + ". ");
								
			if(NumberoftheRound<numberOfRounds){
				System.out.print("Your hardness was " + gameVariables[0] + " and is now ");
				gameVariables[0] = gameVariables[0] * gameVariables[1];
				System.out.println(gameVariables[0] + ".");
								}
			}else{
				System.out.print("Your score is " + gameVariables[2] + ". ");
					if(NumberoftheRound<numberOfRounds){
					System.out.print("Your hardness was " + gameVariables[0] + " and is now ");
							if(gameVariables[0]>5){
								gameVariables[0] = gameVariables[0] / gameVariables[1];
									}
				System.out.println(gameVariables[0] + ".");					
				}				
			    }
				}
						System.out.print("\nThe game is complete. ");
						System.out.println("Your final score was " + gameVariables[2] );
			    }	
		public static int[] getAndCheckStudentAnswer(int[] gameVariables) {
		int Num_1 = (int)(Math.random()*gameVariables[0]);
		int Num_2 = (int)(Math.random()*gameVariables[0]);
		System.out.print("Add " + Num_1 + " and " + Num_2 +": ");
		Scanner get = new Scanner(System.in);
		int studentAnswer = get.nextInt();
			if(studentAnswer == (Num_1 + Num_2)){
				System.out.print("Correct. ");
				gameVariables[3] = 1;
							
			}else{
				System.out.println("Nice try, but the correct answer was " 
				+ (Num_1 + Num_2) + ".");
				gameVariables[3] = 0;
				}
			return gameVariables;
				}
				}
```

##Console
Testing for all correct numbers
```java
Round 1 of 4. Add 2 and 1: 3
Correct. Your score was 0 and is now 5. Your hardness was 5 and is now 10.
Round 2 of 4. Add 3 and 6: 9
Correct. Your score was 5 and is now 15. Your hardness was 10 and is now 20.
Round 3 of 4. Add 12 and 18: 30
Correct. Your score was 15 and is now 35. Your hardness was 20 and is now 40.
Round 4 of 4. Add 12 and 30: 42
Correct. Your score was 35 and is now 75. 
The game is complete. Your final score was 75
```
Testing for all wrong answers
```
Round 1 of 4. Add 1 and 4: 3
Nice try, but the correct answer was 5.
Your score is 0. Your hardness was 5 and is now 5.
Round 2 of 4. Add 4 and 1: 3
Nice try, but the correct answer was 5.
Your score is 0. Your hardness was 5 and is now 5.
Round 3 of 4. Add 4 and 4: 0
Nice try, but the correct answer was 8.
Your score is 0. Your hardness was 5 and is now 5.
Round 4 of 4. Add 0 and 3: 5
Nice try, but the correct answer was 3.
Your score is 0. 
The game is complete. Your final score was 0
```
Testing for two right and two wrong
```
Round 1 of 4. Add 4 and 0: 4
Correct. Your score was 0 and is now 5. Your hardness was 5 and is now 10.
Round 2 of 4. Add 8 and 1: 9
Correct. Your score was 5 and is now 15. Your hardness was 10 and is now 20.
Round 3 of 4. Add 7 and 2: 0
Nice try, but the correct answer was 9.
Your score is 15. Your hardness was 20 and is now 10.
Round 4 of 4. Add 3 and 7: 0
Nice try, but the correct answer was 10.
Your score is 15. 
The game is complete. Your final score was 15
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


