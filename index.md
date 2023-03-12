# Lab Report 5:
### By Daniel Tran

My favorite lab to do was lab 7 where you had to complete a lab task quickly and at the end we would race against other groups in the same lab to see who would finish first. This lab was my favorite because the labs before felt like all I had to do was read and copy the instructions where as this lab I was forced to test my knowledge of previous material in the course to try to figure out a way to do the lab task quickly. The lab itself was not very much reading off a screen and going to previous lab documents and lecture materials to find the right tools to copy and paste and instead it was more of testing our previous knowlege by seeing if we remember how to clone a repository, know how to edit a file within the command line terminal, running JUnit tests on the file and then updating the repository with our new changes.

In this lab, our tasks were as such:
1. Delete any forks of the repository that exist on our account.
2. Fork the repository.
3. Log into ieng6.
4. Clone the repository from our GitHub account
5. Run the JUnit tests on the file and show that they fail.
6. Edit the file(s).
7. Run the JUnit tests again and show that they now all pass.
8. Commit and push the changes on to the repository.

The reason why I enjoyed this lab alot was because it felt more like a skill demo and the fact that I would be racing against my classmates to see who was able to finish these tasks first made the lab that much more fun.

When I was doing the tasks by my self just to see how fast I could do all these tasks, I was going in and just manually typing everything and occasionally using the autocomplete feature to help speed up the process and managed to get in at around 57 seconds to finish the entire task. However when I got together with my group, we discussed how to do the entire lab with other command line tools to do the entire lab in one line. This forces us to use resources like Chat GPT, Stack Overflow, and Geeks for Geeks to see if we can add anything to our line of code to make our group be the fastest. From there we discovered the use of the ```;``` to signify the endline which allowed us to fit other commands into this line and the ```sed``` command which allows us to edit a given file without having to manually go into the file and change the code ourselves.

To use the ```;``` we did something like this in our lab : ```ssh cs15lwi23atd@ieng6.ucsd.edu 'rm -rf lab7/;git clone git@github.com:GonzaloAllenPerez444/lab7.git;cd lab7/;javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar *.java;java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore ListExamplesTest'``` 
where each semicolin would be like a new line in the command line terminal which allowed us to run multiple commands.

To use the ```sed``` command we just added ```sed 's/index1/index2 ListExamples.txt``` which allowed us to quickly edit the file.
In the end our group was able to finsh the task in about 3.5 seconds but when it came time for the race our group could not participate for the final race because there was a copy paste error and we could not figure out why our commands would not work which cost us the win. 


