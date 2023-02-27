# Lab Report 4:
### By Daniel Tran


In this lab report we are going to talk about logging into ieng6, cloning and forking a repository on GitHub, running the junit tests, going into the the file and finding the bug in the code that is producing the error and fixing it, re-running the junit test and committing and pushing the changes to GitHub.

### Step 1: Signing into ieng6
To log into my ieng6 account I typed <ssh cs15lwi23aun@ieng6.ucsd.edu> and pressed <enter> which automatically logged me into the remote server because I added my github ssh key to my account.![Image](/images/terminalSignIn.png)


### Step 2: Forking and cloning from the repository on GitHub
To fork and clone the lab7 repository on GitHub you go to this link [Link](https://github.com/ucsd-cse15l-w23/lab7) which should look like this ![Image](/images/lab7Repo.png) and you go select fork which is this button here ![Image](/images/fork.png) and you press fork.
To clone you then press the code button which looks like this [Image]!(clone.png) and press it where you go to ssh instead of the normal clone which looks like this: ![Image](/images/clone.png)
  and you go here: ![Image](/images/sshClone.png) 
  and this will give you a link where you will paste it into ieng6. In my case the link looks like this git@github.com:dtran556/lab7.git and you go back to the terminal and type this <git clone git@github.com:dtran556/lab7.git> and press <enter> and it looks like this ![Image](/images/terminalClone.png).


### Step 3: Running the JUnit tests
Next we are running the Junit tests. You type this: <cd lab7> <enter> <ls> <javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar *.java> and if you do not get any compile errors you press this: <java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore ListExamplesTest> which will tell you if you passed the tests or not. In the case of the lab it should look like this : ![Image](/images/failTestClone.png).


### Step 4: Going into the java file and editing the code
Since the Junit tests failed we need to go into the file and edit the code so that it will pass the Junit tests. You then type <nano ListExamples.java> looked for the bug and then type< ^W index2> to jump to the bug and then edit the code and then press <^O> to save and then <^X> <enter> to save and exit.


### Step 5: Running the Junit tests again
  To run the Junit tests again you can use the history of the terminal and press <up> on the key pad until you find the javac command to compile the files and the junit test and press the <up> key again until you see the java command from step 3 and check to see if the edits worked.


### Step 6: Commiting and pushing on to GitHub
  If the edits worked and you want to push it onto GitHub you type <git add ListExamples.java> and press <enter> then you type <git commit -m "your choice of message here"> and press <enter> and then type <git push> and press <enter> and you have successfully commited and pushed your edits onto GitHub
