# Lab Report 5:
### By Daniel Tran


Today we will be talking about the command line command `grep` and its different uses. We will be using the written_2 directory from week 4 lab.


## Command line command : `grep -r ""`
The `grep -r ""` command allows you to go into a directory and find the path that contains the string arguement that the user passes in and provide the context in which the string was mentioned
Example 1: 


Example 2:

## Command line command #2 `grep -c "" `
This command allows you to go through one or more files to check to see how many times a word appears in each file.
Example 1 looking at one file:


Example 2 looking through multiple files :


## Command line command #3 `grep -v ""`
wi23aun@ieng6-201]:Abernathy:352$ grep -c "titan" ch1.txt
0

## Command line command #4 `grep -l ""`
You can use this command to look for a given string inside files in a directory.

Example 1 looking for a string inside one directory:

Example 2 using -l with -r to look through multiple directories:


To find these commands I found this website which had most of the commands : [Reference to Commands]([https://link-url-here.org](https://docs.rackspace.com/support/how-to/use-the-linux-grep-command/)) and I also looked at ``` man grep``` for a list of commands.



