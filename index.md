# Lab Report 4:
### By Daniel Tran


In this lab report we are going to talk about logging into ieng6, cloning and forking a repository on GitHub, running the junit tests, going into the the file and finding the bug in the code that is producing the error and fixing it, re-running the junit test and committing and pushing the changes to GitHub.

### Step 1: Signing into ieng6
To log into my ieng6 account I typed <ssh cs15lwi23aun@ieng6.ucsd.edu> and pressed <enter> which automatically logged me into the remote server because I added my github ssh key to my account.[Image]!(terminalSignIn.png)


### Step 2: Forking and cloning from the repository on GitHub
To fork and clone the lab7 repository on GitHub you go to this link [Link]!(https://github.com/ucsd-cse15l-w23/lab7) which should look like this [Image]!(lab7Repo.png) and you go select fork which is this button here [Image]!(fork.png) and you press fork.
To clone you then press the code button which looks like this [Image]!(clone.png) and press it where you go to ssh instead of the normal clone which looks like this [Image]!(normalClone.png) and you go here [Image]!(sshClone.png) and this will give you a link where you will paste it into ieng6. In my case the link looks like this git@github.com:dtran556/lab7.git and you go back to the terminal and type this < git clone git@github.com:dtran556/lab7.git> and press <enter> and it looks like this [Image]!(terminalClone.png).


### Step 3: Running the JUnit tests
Next we are running the Junit tests. You type this: <javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar *.java> and if you do not get any compile errors you press this: <java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore ListExamplesTest> which will tell you if you passed the tests or not. In the case of the lab it should look like this : Image]!(failTestClone.png).


### Step 4: Going into the java file and editing the code


### Step 5: Running the Junit tests again


### Step 6: Commiting and pushing on to GitHub
