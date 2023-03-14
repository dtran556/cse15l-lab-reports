# Lab Report 5:
### By Daniel Tran


Today we will be talking about the command line command ```find``` and its different uses. We will be using the written_2 directory from week 4 lab.


## Command line command : `find [path] -type f -name "FileName`
The `grep -r ""` command allows you to go into a directory and find the path that contains the string arguement that the user passes in and provide the context in which the string was mentioned

This find command will look for the specified file names because of the `-type f` which is basically telling the computer to only look for files and the `-name` portion tells the computer to look for the files with the provided name. 
Example 1: 
```
[cs15lwi23aun@ieng6-201]:~:501$ ls   
docsearch  hello.txt  lab1  lab7  list-examples-grader  perl5  skill-demo1-data  skill-demo1-server  wavelet
[cs15lwi23aun@ieng6-201]:~:502$ cd skill-demo1-data
[cs15lwi23aun@ieng6-201]:skill-demo1-data:503$ cd written_2
[cs15lwi23aun@ieng6-201]:written_2:504$ find -f
find: unknown predicate `-f'
[cs15lwi23aun@ieng6-201]:written_2:505$ find -type      
find: missing argument to `-type'
[cs15lwi23aun@ieng6-201]:written_2:506$ find written_2 -type f -name "*.txt"
find: 'written_2': No such file or directory
[cs15lwi23aun@ieng6-201]:written_2:507$ cd ..
[cs15lwi23aun@ieng6-201]:skill-demo1-data:508$ find written_2 -type f -name "*.txt"
written_2/non-fiction/OUP/Abernathy/ch1.txt
written_2/non-fiction/OUP/Abernathy/ch14.txt
written_2/non-fiction/OUP/Abernathy/ch15.txt
written_2/non-fiction/OUP/Abernathy/ch2.txt
written_2/non-fiction/OUP/Abernathy/ch3.txt
written_2/non-fiction/OUP/Abernathy/ch6.txt
written_2/non-fiction/OUP/Abernathy/ch7.txt
written_2/non-fiction/OUP/Abernathy/ch8.txt
written_2/non-fiction/OUP/Abernathy/ch9.txt
written_2/non-fiction/OUP/Berk/CH4.txt
written_2/non-fiction/OUP/Berk/ch1.txt
written_2/non-fiction/OUP/Berk/ch2.txt
written_2/non-fiction/OUP/Berk/ch7.txt
written_2/non-fiction/OUP/Castro/chA.txt
written_2/non-fiction/OUP/Castro/chB.txt
written_2/non-fiction/OUP/Castro/chC.txt
written_2/non-fiction/OUP/Castro/chL.txt
written_2/non-fiction/OUP/Castro/chM.txt
written_2/non-fiction/OUP/Castro/chN.txt
written_2/non-fiction/OUP/Castro/chO.txt
written_2/non-fiction/OUP/Castro/chP.txt
written_2/non-fiction/OUP/Castro/chQ.txt
written_2/non-fiction/OUP/Castro/chR.txt
written_2/non-fiction/OUP/Castro/chV.txt
written_2/non-fiction/OUP/Castro/chW.txt
written_2/non-fiction/OUP/Castro/chY.txt
written_2/non-fiction/OUP/Castro/chZ.txt
written_2/non-fiction/OUP/Fletcher/ch1.txt
written_2/non-fiction/OUP/Fletcher/ch10.txt
written_2/non-fiction/OUP/Fletcher/ch2.txt
written_2/non-fiction/OUP/Fletcher/ch5.txt
written_2/non-fiction/OUP/Fletcher/ch6.txt
written_2/non-fiction/OUP/Fletcher/ch9.txt
written_2/non-fiction/OUP/Kauffman/ch1.txt
written_2/non-fiction/OUP/Kauffman/ch10.txt
written_2/non-fiction/OUP/Kauffman/ch3.txt
written_2/non-fiction/OUP/Kauffman/ch4.txt
written_2/non-fiction/OUP/Kauffman/ch5.txt
written_2/non-fiction/OUP/Kauffman/ch6.txt
written_2/non-fiction/OUP/Kauffman/ch7.txt
written_2/non-fiction/OUP/Kauffman/ch8.txt
written_2/non-fiction/OUP/Kauffman/ch9.txt
written_2/non-fiction/OUP/Rybczynski/ch1.txt
written_2/non-fiction/OUP/Rybczynski/ch2.txt
written_2/non-fiction/OUP/Rybczynski/ch3.txt
written_2/travel_guides/berlitz1/HandRHawaii.txt
written_2/travel_guides/berlitz1/HandRHongKong.txt
written_2/travel_guides/berlitz1/HandRIbiza.txt
written_2/travel_guides/berlitz1/HandRIsrael.txt
written_2/travel_guides/berlitz1/HandRIstanbul.txt
written_2/travel_guides/berlitz1/HandRJamaica.txt
written_2/travel_guides/berlitz1/HandRJerusalem.txt
written_2/travel_guides/berlitz1/HandRLakeDistrict.txt
written_2/travel_guides/berlitz1/HandRLasVegas.txt
written_2/travel_guides/berlitz1/HandRLisbon.txt
written_2/travel_guides/berlitz1/HandRLosAngeles.txt
written_2/travel_guides/berlitz1/HandRMadeira.txt
written_2/travel_guides/berlitz1/HandRMadrid.txt
written_2/travel_guides/berlitz1/HandRMallorca.txt
written_2/travel_guides/berlitz1/HistoryDublin.txt
written_2/travel_guides/berlitz1/HistoryEdinburgh.txt
written_2/travel_guides/berlitz1/HistoryEgypt.txt
written_2/travel_guides/berlitz1/HistoryFWI.txt
written_2/travel_guides/berlitz1/HistoryFrance.txt
written_2/travel_guides/berlitz1/HistoryGreek.txt
written_2/travel_guides/berlitz1/HistoryHawaii.txt
written_2/travel_guides/berlitz1/HistoryHongKong.txt
written_2/travel_guides/berlitz1/HistoryIbiza.txt
written_2/travel_guides/berlitz1/HistoryIndia.txt
written_2/travel_guides/berlitz1/HistoryIsrael.txt
written_2/travel_guides/berlitz1/HistoryIstanbul.txt
written_2/travel_guides/berlitz1/HistoryItaly.txt
written_2/travel_guides/berlitz1/HistoryJamaica.txt
written_2/travel_guides/berlitz1/HistoryJapan.txt
written_2/travel_guides/berlitz1/HistoryJerusalem.txt
written_2/travel_guides/berlitz1/HistoryLakeDistrict.txt
written_2/travel_guides/berlitz1/HistoryLasVegas.txt
written_2/travel_guides/berlitz1/HistoryMadeira.txt
written_2/travel_guides/berlitz1/HistoryMadrid.txt
written_2/travel_guides/berlitz1/HistoryMalaysia.txt
written_2/travel_guides/berlitz1/HistoryMallorca.txt
written_2/travel_guides/berlitz1/IntroDublin.txt
written_2/travel_guides/berlitz1/IntroEdinburgh.txt
written_2/travel_guides/berlitz1/IntroEgypt.txt
written_2/travel_guides/berlitz1/IntroFWI.txt
written_2/travel_guides/berlitz1/IntroFrance.txt
written_2/travel_guides/berlitz1/IntroGreek.txt
written_2/travel_guides/berlitz1/IntroHongKong.txt
written_2/travel_guides/berlitz1/IntroIbiza.txt
written_2/travel_guides/berlitz1/IntroIndia.txt
written_2/travel_guides/berlitz1/IntroIsrael.txt
written_2/travel_guides/berlitz1/IntroIstanbul.txt
written_2/travel_guides/berlitz1/IntroItaly.txt
written_2/travel_guides/berlitz1/IntroJamaica.txt
written_2/travel_guides/berlitz1/IntroJapan.txt
written_2/travel_guides/berlitz1/IntroJerusalem.txt
written_2/travel_guides/berlitz1/IntroLakeDistrict.txt
written_2/travel_guides/berlitz1/IntroLasVegas.txt
written_2/travel_guides/berlitz1/IntroLosAngeles.txt
written_2/travel_guides/berlitz1/IntroMadeira.txt
written_2/travel_guides/berlitz1/IntroMadrid.txt
written_2/travel_guides/berlitz1/IntroMalaysia.txt
written_2/travel_guides/berlitz1/IntroMallorca.txt
written_2/travel_guides/berlitz1/JungleMalaysia.txt
written_2/travel_guides/berlitz1/WhatToDublin.txt
written_2/travel_guides/berlitz1/WhatToEdinburgh.txt
written_2/travel_guides/berlitz1/WhatToEgypt.txt
written_2/travel_guides/berlitz1/WhatToFWI.txt
written_2/travel_guides/berlitz1/WhatToFrance.txt
written_2/travel_guides/berlitz1/WhatToGreek.txt
written_2/travel_guides/berlitz1/WhatToHawaii.txt
written_2/travel_guides/berlitz1/WhatToHongKong.txt
written_2/travel_guides/berlitz1/WhatToIbiza.txt
written_2/travel_guides/berlitz1/WhatToIndia.txt
written_2/travel_guides/berlitz1/WhatToIsrael.txt
written_2/travel_guides/berlitz1/WhatToIstanbul.txt
written_2/travel_guides/berlitz1/WhatToItaly.txt
written_2/travel_guides/berlitz1/WhatToJamaica.txt
written_2/travel_guides/berlitz1/WhatToJapan.txt
written_2/travel_guides/berlitz1/WhatToLakeDistrict.txt
written_2/travel_guides/berlitz1/WhatToLasVegas.txt
written_2/travel_guides/berlitz1/WhatToLosAngeles.txt
written_2/travel_guides/berlitz1/WhatToMadeira.txt
written_2/travel_guides/berlitz1/WhatToMalaysia.txt
written_2/travel_guides/berlitz1/WhatToMallorca.txt
written_2/travel_guides/berlitz1/WhereToDublin.txt
written_2/travel_guides/berlitz1/WhereToEdinburgh.txt
written_2/travel_guides/berlitz1/WhereToEgypt.txt
written_2/travel_guides/berlitz1/WhereToFWI.txt
written_2/travel_guides/berlitz1/WhereToFrance.txt
written_2/travel_guides/berlitz1/WhereToGreek.txt
written_2/travel_guides/berlitz1/WhereToHawaii.txt
written_2/travel_guides/berlitz1/WhereToHongKong.txt
written_2/travel_guides/berlitz1/WhereToIbiza.txt
written_2/travel_guides/berlitz1/WhereToIndia.txt
written_2/travel_guides/berlitz1/WhereToIsrael.txt
written_2/travel_guides/berlitz1/WhereToIstanbul.txt
written_2/travel_guides/berlitz1/WhereToItaly.txt
written_2/travel_guides/berlitz1/WhereToJapan.txt
written_2/travel_guides/berlitz1/WhereToJerusalem.txt
written_2/travel_guides/berlitz1/WhereToLakeDistrict.txt
written_2/travel_guides/berlitz1/WhereToLosAngeles.txt
written_2/travel_guides/berlitz1/WhereToMadeira.txt
written_2/travel_guides/berlitz1/WhereToMadrid.txt
written_2/travel_guides/berlitz1/WhereToMalaysia.txt
written_2/travel_guides/berlitz1/WhereToMallorca.txt
written_2/travel_guides/berlitz2/Algarve-History.txt
written_2/travel_guides/berlitz2/Algarve-Intro.txt
written_2/travel_guides/berlitz2/Algarve-WhatToDo.txt
written_2/travel_guides/berlitz2/Algarve-WhereToGo.txt
written_2/travel_guides/berlitz2/Amsterdam-History.txt
written_2/travel_guides/berlitz2/Amsterdam-Intro.txt
written_2/travel_guides/berlitz2/Amsterdam-WhatToDo.txt
written_2/travel_guides/berlitz2/Amsterdam-WhereToGo.txt
written_2/travel_guides/berlitz2/Athens-History.txt
written_2/travel_guides/berlitz2/Athens-Intro.txt
written_2/travel_guides/berlitz2/Athens-WhatToDo.txt
written_2/travel_guides/berlitz2/Athens-WhereToGo.txt
written_2/travel_guides/berlitz2/Bahamas-History.txt
written_2/travel_guides/berlitz2/Bahamas-Intro.txt
written_2/travel_guides/berlitz2/Bahamas-WhatToDo.txt
written_2/travel_guides/berlitz2/Bahamas-WhereToGo.txt
written_2/travel_guides/berlitz2/Bali-History.txt
written_2/travel_guides/berlitz2/Bali-WhatToDo.txt
written_2/travel_guides/berlitz2/Bali-WhereToGo.txt
written_2/travel_guides/berlitz2/Barcelona-History.txt
written_2/travel_guides/berlitz2/Barcelona-WhatToDo.txt
written_2/travel_guides/berlitz2/Barcelona-WhereToGo.txt
written_2/travel_guides/berlitz2/Beijing-History.txt
written_2/travel_guides/berlitz2/Beijing-WhatToDo.txt
written_2/travel_guides/berlitz2/Beijing-WhereToGo.txt
written_2/travel_guides/berlitz2/Berlin-History.txt
written_2/travel_guides/berlitz2/Berlin-WhatToDo.txt
written_2/travel_guides/berlitz2/Berlin-WhereToGo.txt
written_2/travel_guides/berlitz2/Bermuda-WhatToDo.txt
written_2/travel_guides/berlitz2/Bermuda-WhereToGo.txt
written_2/travel_guides/berlitz2/Bermuda-history.txt
written_2/travel_guides/berlitz2/Boston-WhereToGo.txt
written_2/travel_guides/berlitz2/Budapest-History.txt
written_2/travel_guides/berlitz2/Budapest-WhatToDo.txt
written_2/travel_guides/berlitz2/Budapest-WhereoGo.txt
written_2/travel_guides/berlitz2/California-History.txt
written_2/travel_guides/berlitz2/California-WhatToDo.txt
written_2/travel_guides/berlitz2/California-WhereToGo.txt
written_2/travel_guides/berlitz2/Canada-History.txt
written_2/travel_guides/berlitz2/Canada-WhereToGo.txt
written_2/travel_guides/berlitz2/CanaryIslands-History.txt
written_2/travel_guides/berlitz2/CanaryIslands-WhatToDo.txt
written_2/travel_guides/berlitz2/CanaryIslands-WhereToGo.txt
written_2/travel_guides/berlitz2/Cancun-History.txt
written_2/travel_guides/berlitz2/Cancun-WhatToDo.txt
written_2/travel_guides/berlitz2/Cancun-WhereToGo.txt
written_2/travel_guides/berlitz2/China-History.txt
written_2/travel_guides/berlitz2/China-WhatToDo.txt
written_2/travel_guides/berlitz2/China-WhereToGo.txt
written_2/travel_guides/berlitz2/Costa-History.txt
written_2/travel_guides/berlitz2/Costa-WhatToDo.txt
written_2/travel_guides/berlitz2/Costa-WhereToGo.txt
written_2/travel_guides/berlitz2/CostaBlanca-History.txt
written_2/travel_guides/berlitz2/CostaBlanca-WhatToDo.txt
written_2/travel_guides/berlitz2/Crete-History.txt
written_2/travel_guides/berlitz2/Crete-WhatToDo.txt
written_2/travel_guides/berlitz2/Crete-WhereToGo.txt
written_2/travel_guides/berlitz2/CstaBlanca-WhereToGo.txt
written_2/travel_guides/berlitz2/Cuba-History.txt
written_2/travel_guides/berlitz2/Cuba-WhatToDo.txt
written_2/travel_guides/berlitz2/Cuba-WhereToGo.txt
written_2/travel_guides/berlitz2/Nepal-History.txt
written_2/travel_guides/berlitz2/Nepal-WhatToDo.txt
written_2/travel_guides/berlitz2/Nepal-WhereToGo.txt
written_2/travel_guides/berlitz2/NewOrleans-History.txt
written_2/travel_guides/berlitz2/Paris-WhatToDo.txt
written_2/travel_guides/berlitz2/Paris-WhereToGo.txt
written_2/travel_guides/berlitz2/Poland-History.txt
written_2/travel_guides/berlitz2/Poland-WhatToDo.txt
written_2/travel_guides/berlitz2/Portugal-History.txt
written_2/travel_guides/berlitz2/Portugal-WhatToDo.txt
written_2/travel_guides/berlitz2/Portugal-WhereToGo.txt
written_2/travel_guides/berlitz2/PuertoRico-History.txt
written_2/travel_guides/berlitz2/PuertoRico-WhatToDo.txt
written_2/travel_guides/berlitz2/PuertoRico-WhereToGo.txt
written_2/travel_guides/berlitz2/Vallarta-History.txt
written_2/travel_guides/berlitz2/Vallarta-WhatToDo.txt
written_2/travel_guides/berlitz2/Vallarta-WhereToGo.txt
[cs15lwi23aun@ieng6-201]:skill-demo1-data:509$ 
```

In the example above I am basically asking the computer to go into the `written_2` directory and find me all of the files and tell me its file pathing.

Example 2:
```
[cs15lwi23aun@ieng6-201]:skill-demo1-data:509$ find written_2 -type f -name "Bahamas-History.txt"
written_2/travel_guides/berlitz2/Bahamas-History.txt
[cs15lwi23aun@ieng6-201]:skill-demo1-data:510$ 
```
In the example above I ask the computer to look for a file called `Bahamas-History.txt` and it returns the file and its file pathing.

## Command line command #2 ` find [path] -iname ""` 
Lets say you want to find a file but cannot remember the exact name of the file you can use `-iname` where it ignores the cases in the file name you gave the computer.

Example 1 looking at one file:
```
[cs15lwi23aun@ieng6-201]:skill-demo1-data:511$  find written_2  -iname "bAhaMaS-HiStOrY.txt"
written_2/travel_guides/berlitz2/Bahamas-History.txt
```
In this example I am looking for the file named `Bahamas-History.txt` but I purposely messed up the cases and used the `-iname` command to ignore the cases so it would still find me a file with the same characters.

Example 2 looking through multiple files :
```
[cs15lwi23aun@ieng6-201]:skill-demo1-data:512$  find written_2  -iname "*cH*.txt"
written_2/non-fiction/OUP/Abernathy/ch1.txt
written_2/non-fiction/OUP/Abernathy/ch14.txt
written_2/non-fiction/OUP/Abernathy/ch15.txt
written_2/non-fiction/OUP/Abernathy/ch2.txt
written_2/non-fiction/OUP/Abernathy/ch3.txt
written_2/non-fiction/OUP/Abernathy/ch6.txt
written_2/non-fiction/OUP/Abernathy/ch7.txt
written_2/non-fiction/OUP/Abernathy/ch8.txt
written_2/non-fiction/OUP/Abernathy/ch9.txt
written_2/non-fiction/OUP/Berk/CH4.txt
written_2/non-fiction/OUP/Berk/ch1.txt
written_2/non-fiction/OUP/Berk/ch2.txt
written_2/non-fiction/OUP/Berk/ch7.txt
written_2/non-fiction/OUP/Castro/chA.txt
written_2/non-fiction/OUP/Castro/chB.txt
written_2/non-fiction/OUP/Castro/chC.txt
written_2/non-fiction/OUP/Castro/chL.txt
written_2/non-fiction/OUP/Castro/chM.txt
written_2/non-fiction/OUP/Castro/chN.txt
written_2/non-fiction/OUP/Castro/chO.txt
written_2/non-fiction/OUP/Castro/chP.txt
written_2/non-fiction/OUP/Castro/chQ.txt
written_2/non-fiction/OUP/Castro/chR.txt
written_2/non-fiction/OUP/Castro/chV.txt
written_2/non-fiction/OUP/Castro/chW.txt
written_2/non-fiction/OUP/Castro/chY.txt
written_2/non-fiction/OUP/Castro/chZ.txt
written_2/non-fiction/OUP/Fletcher/ch1.txt
written_2/non-fiction/OUP/Fletcher/ch10.txt
written_2/non-fiction/OUP/Fletcher/ch2.txt
written_2/non-fiction/OUP/Fletcher/ch5.txt
written_2/non-fiction/OUP/Fletcher/ch6.txt
written_2/non-fiction/OUP/Fletcher/ch9.txt
written_2/non-fiction/OUP/Kauffman/ch1.txt
written_2/non-fiction/OUP/Kauffman/ch10.txt
written_2/non-fiction/OUP/Kauffman/ch3.txt
written_2/non-fiction/OUP/Kauffman/ch4.txt
written_2/non-fiction/OUP/Kauffman/ch5.txt
written_2/non-fiction/OUP/Kauffman/ch6.txt
written_2/non-fiction/OUP/Kauffman/ch7.txt
written_2/non-fiction/OUP/Kauffman/ch8.txt
written_2/non-fiction/OUP/Kauffman/ch9.txt
written_2/non-fiction/OUP/Rybczynski/ch1.txt
written_2/non-fiction/OUP/Rybczynski/ch2.txt
written_2/non-fiction/OUP/Rybczynski/ch3.txt
written_2/travel_guides/berlitz2/China-History.txt
written_2/travel_guides/berlitz2/China-WhatToDo.txt
written_2/travel_guides/berlitz2/China-WhereToGo.txt
[cs15lwi23aun@ieng6-201]:skill-demo1-data:513$ 
```
In the example above I am basically asking the computer to go into the `written_2` directory and find me all of the files and its pathing however I used the `*`  to tell the computer to look for every .txt file and every file with the charcters "Ch" in them.


## Command line command #3 `find [path] -ls`
This command will recursively look for everything inside a directory and will list it out. 
Example :
```
[cs15lwi23aun@ieng6-201]:skill-demo1-data:513$ find written_2 -ls
202637392    4 drwxr-s---   4 cs15lwi23aun ieng6_cs15lwi23     4096 Feb  8 18:47 written_2
202637409    4 drwxr-s---   3 cs15lwi23aun ieng6_cs15lwi23     4096 Feb  8 18:47 written_2/non-fiction
202637410    4 drwxr-s---   8 cs15lwi23aun ieng6_cs15lwi23     4096 Feb  8 18:47 written_2/non-fiction/OUP
202637411    4 drwxr-s---   2 cs15lwi23aun ieng6_cs15lwi23     4096 Feb  8 18:47 written_2/non-fiction/OUP/Abernathy
202637412   52 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    46915 Feb  8 18:47 written_2/non-fiction/OUP/Abernathy/ch1.txt
202637413   44 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    39905 Feb  8 18:47 written_2/non-fiction/OUP/Abernathy/ch14.txt
202637397   48 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    43918 Feb  8 18:47 written_2/non-fiction/OUP/Abernathy/ch15.txt
202637414   48 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    44782 Feb  8 18:47 written_2/non-fiction/OUP/Abernathy/ch2.txt
202637415   40 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    35141 Feb  8 18:47 written_2/non-fiction/OUP/Abernathy/ch3.txt
202637416   48 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    42225 Feb  8 18:47 written_2/non-fiction/OUP/Abernathy/ch6.txt
202637417   48 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    42444 Feb  8 18:47 written_2/non-fiction/OUP/Abernathy/ch7.txt
202637418   56 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    52468 Feb  8 18:47 written_2/non-fiction/OUP/Abernathy/ch8.txt
202637419   36 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    31283 Feb  8 18:47 written_2/non-fiction/OUP/Abernathy/ch9.txt
202637420    4 drwxr-s---   2 cs15lwi23aun ieng6_cs15lwi23     4096 Feb  8 18:47 written_2/non-fiction/OUP/Berk
202637421  108 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23   103491 Feb  8 18:47 written_2/non-fiction/OUP/Berk/CH4.txt
202637422   96 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    92355 Feb  8 18:47 written_2/non-fiction/OUP/Berk/ch1.txt
202637423  108 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23   102942 Feb  8 18:47 written_2/non-fiction/OUP/Berk/ch2.txt
202637424   72 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    66887 Feb  8 18:47 written_2/non-fiction/OUP/Berk/ch7.txt
202637425    4 drwxr-s---   2 cs15lwi23aun ieng6_cs15lwi23     4096 Feb  8 18:47 written_2/non-fiction/OUP/Castro
202637426   40 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    35675 Feb  8 18:47 written_2/non-fiction/OUP/Castro/chA.txt
202637427   40 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    32819 Feb  8 18:47 written_2/non-fiction/OUP/Castro/chB.txt
202637428   28 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    23635 Feb  8 18:47 written_2/non-fiction/OUP/Castro/chC.txt
202637429   28 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    24476 Feb  8 18:47 written_2/non-fiction/OUP/Castro/chL.txt
202637430   60 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    55410 Feb  8 18:47 written_2/non-fiction/OUP/Castro/chM.txt
202637431   12 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23     9182 Feb  8 18:47 written_2/non-fiction/OUP/Castro/chN.txt
202637432   12 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23     8349 Feb  8 18:47 written_2/non-fiction/OUP/Castro/chO.txt
202637433   48 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    41470 Feb  8 18:47 written_2/non-fiction/OUP/Castro/chP.txt
202637434   12 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23     8274 Feb  8 18:47 written_2/non-fiction/OUP/Castro/chQ.txt
202637436   40 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    33420 Feb  8 18:47 written_2/non-fiction/OUP/Castro/chR.txt
202637437   20 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    19909 Feb  8 18:47 written_2/non-fiction/OUP/Castro/chV.txt
202637438    8 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23     6724 Feb  8 18:47 written_2/non-fiction/OUP/Castro/chW.txt
202637439    8 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23     5424 Feb  8 18:47 written_2/non-fiction/OUP/Castro/chY.txt
202637440    8 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23     5431 Feb  8 18:47 written_2/non-fiction/OUP/Castro/chZ.txt
202637441    4 drwxr-s---   2 cs15lwi23aun ieng6_cs15lwi23     4096 Feb  8 18:47 written_2/non-fiction/OUP/Fletcher
202637442   52 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    46376 Feb  8 18:47 written_2/non-fiction/OUP/Fletcher/ch1.txt
202637443   40 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    33013 Feb  8 18:47 written_2/non-fiction/OUP/Fletcher/ch10.txt
202637444   56 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    51325 Feb  8 18:47 written_2/non-fiction/OUP/Fletcher/ch2.txt
202637445   52 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    48389 Feb  8 18:47 written_2/non-fiction/OUP/Fletcher/ch5.txt
202637446   72 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    68106 Feb  8 18:47 written_2/non-fiction/OUP/Fletcher/ch6.txt
202637447   60 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    53257 Feb  8 18:47 written_2/non-fiction/OUP/Fletcher/ch9.txt
202637450    4 drwxr-s---   2 cs15lwi23aun ieng6_cs15lwi23     4096 Feb  8 18:47 written_2/non-fiction/OUP/Kauffman
202637451   72 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    65578 Feb  8 18:47 written_2/non-fiction/OUP/Kauffman/ch1.txt
202637452   68 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    64908 Feb  8 18:47 written_2/non-fiction/OUP/Kauffman/ch10.txt
202637453   84 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    80544 Feb  8 18:47 written_2/non-fiction/OUP/Kauffman/ch3.txt
202637454   80 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    74448 Feb  8 18:47 written_2/non-fiction/OUP/Kauffman/ch4.txt
202637455   32 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    27196 Feb  8 18:47 written_2/non-fiction/OUP/Kauffman/ch5.txt
202637456   68 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    61513 Feb  8 18:47 written_2/non-fiction/OUP/Kauffman/ch6.txt
202637457   56 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    50095 Feb  8 18:47 written_2/non-fiction/OUP/Kauffman/ch7.txt
202637458  104 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    99145 Feb  8 18:47 written_2/non-fiction/OUP/Kauffman/ch8.txt
202637459   92 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    86220 Feb  8 18:47 written_2/non-fiction/OUP/Kauffman/ch9.txt
202637460    4 drwxr-s---   2 cs15lwi23aun ieng6_cs15lwi23     4096 Feb  8 18:47 written_2/non-fiction/OUP/Rybczynski
202637461   40 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    34412 Feb  8 18:47 written_2/non-fiction/OUP/Rybczynski/ch1.txt
202637462   44 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    38052 Feb  8 18:47 written_2/non-fiction/OUP/Rybczynski/ch2.txt
202637435   56 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    52179 Feb  8 18:47 written_2/non-fiction/OUP/Rybczynski/ch3.txt
202637448    4 drwxr-s---   4 cs15lwi23aun ieng6_cs15lwi23     4096 Feb  8 18:47 written_2/travel_guides
202637449    8 drwxr-s---   2 cs15lwi23aun ieng6_cs15lwi23     8192 Feb  8 18:47 written_2/travel_guides/berlitz1
202637463   16 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    16271 Feb  8 18:47 written_2/travel_guides/berlitz1/HandRHawaii.txt
202637464    4 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23     1193 Feb  8 18:47 written_2/travel_guides/berlitz1/HandRHongKong.txt
202637465    4 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23      675 Feb  8 18:47 written_2/travel_guides/berlitz1/HandRIbiza.txt
202637466   32 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    25689 Feb  8 18:47 written_2/travel_guides/berlitz1/HandRIsrael.txt
202637467    4 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23      931 Feb  8 18:47 written_2/travel_guides/berlitz1/HandRIstanbul.txt
202637468   32 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    25434 Feb  8 18:47 written_2/travel_guides/berlitz1/HandRJamaica.txt
202637469    4 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23     1446 Feb  8 18:47 written_2/travel_guides/berlitz1/HandRJerusalem.txt
202637470    4 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23     1528 Feb  8 18:47 written_2/travel_guides/berlitz1/HandRLakeDistrict.txt
202637471    4 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23     1547 Feb  8 18:47 written_2/travel_guides/berlitz1/HandRLasVegas.txt
202637472    4 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23     1067 Feb  8 18:47 written_2/travel_guides/berlitz1/HandRLisbon.txt
202637473    4 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23     1254 Feb  8 18:47 written_2/travel_guides/berlitz1/HandRLosAngeles.txt
202637474    4 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23     1433 Feb  8 18:47 written_2/travel_guides/berlitz1/HandRMadeira.txt
202637475   16 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    14092 Feb  8 18:47 written_2/travel_guides/berlitz1/HandRMadrid.txt
202637476    4 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23     1445 Feb  8 18:47 written_2/travel_guides/berlitz1/HandRMallorca.txt
202637477   16 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    15962 Feb  8 18:47 written_2/travel_guides/berlitz1/HistoryDublin.txt
202637478   28 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    21027 Feb  8 18:47 written_2/travel_guides/berlitz1/HistoryEdinburgh.txt
202637479   20 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    18298 Feb  8 18:47 written_2/travel_guides/berlitz1/HistoryEgypt.txt
202637480   16 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    15011 Feb  8 18:47 written_2/travel_guides/berlitz1/HistoryFWI.txt
202637481   44 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    38509 Feb  8 18:47 written_2/travel_guides/berlitz1/HistoryFrance.txt
202637482   20 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    18666 Feb  8 18:47 written_2/travel_guides/berlitz1/HistoryGreek.txt
202637483   20 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    16522 Feb  8 18:47 written_2/travel_guides/berlitz1/HistoryHawaii.txt
202637484   16 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    14614 Feb  8 18:47 written_2/travel_guides/berlitz1/HistoryHongKong.txt
202637485   16 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    12703 Feb  8 18:47 written_2/travel_guides/berlitz1/HistoryIbiza.txt
202637486   60 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    54898 Feb  8 18:47 written_2/travel_guides/berlitz1/HistoryIndia.txt
202637487   20 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    16573 Feb  8 18:47 written_2/travel_guides/berlitz1/HistoryIsrael.txt
202637488   32 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    27099 Feb  8 18:47 written_2/travel_guides/berlitz1/HistoryIstanbul.txt
202637489   52 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    48191 Feb  8 18:47 written_2/travel_guides/berlitz1/HistoryItaly.txt
202637490   20 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    17168 Feb  8 18:47 written_2/travel_guides/berlitz1/HistoryJamaica.txt
202637491   48 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    41789 Feb  8 18:47 written_2/travel_guides/berlitz1/HistoryJapan.txt
202637492   20 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    18491 Feb  8 18:47 written_2/travel_guides/berlitz1/HistoryJerusalem.txt
202637493   16 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    13596 Feb  8 18:47 written_2/travel_guides/berlitz1/HistoryLakeDistrict.txt
202637494   20 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    18968 Feb  8 18:47 written_2/travel_guides/berlitz1/HistoryLasVegas.txt
202637496   12 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    11857 Feb  8 18:47 written_2/travel_guides/berlitz1/HistoryMadeira.txt
202637497   16 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    12519 Feb  8 18:47 written_2/travel_guides/berlitz1/HistoryMadrid.txt
202637499   40 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    35725 Feb  8 18:47 written_2/travel_guides/berlitz1/HistoryMalaysia.txt
202637500   16 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    13730 Feb  8 18:47 written_2/travel_guides/berlitz1/HistoryMallorca.txt
202637502    8 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23     7820 Feb  8 18:47 written_2/travel_guides/berlitz1/IntroDublin.txt
202637503   12 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23     9427 Feb  8 18:47 written_2/travel_guides/berlitz1/IntroEdinburgh.txt
202637504    8 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23     7989 Feb  8 18:47 written_2/travel_guides/berlitz1/IntroEgypt.txt
202637506    8 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23     7684 Feb  8 18:47 written_2/travel_guides/berlitz1/IntroFWI.txt
202637507   12 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    11010 Feb  8 18:47 written_2/travel_guides/berlitz1/IntroFrance.txt
202637509   12 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23     8323 Feb  8 18:47 written_2/travel_guides/berlitz1/IntroGreek.txt
202637510    8 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23     5784 Feb  8 18:47 written_2/travel_guides/berlitz1/IntroHongKong.txt
202637511    8 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23     6210 Feb  8 18:47 written_2/travel_guides/berlitz1/IntroIbiza.txt
202637513   32 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    26436 Feb  8 18:47 written_2/travel_guides/berlitz1/IntroIndia.txt
202640876    8 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23     5318 Feb  8 18:47 written_2/travel_guides/berlitz1/IntroIsrael.txt
202642879    8 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23     7212 Feb  8 18:47 written_2/travel_guides/berlitz1/IntroIstanbul.txt
202643121   16 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    12345 Feb  8 18:47 written_2/travel_guides/berlitz1/IntroItaly.txt
202644603   12 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    10468 Feb  8 18:47 written_2/travel_guides/berlitz1/IntroJamaica.txt
202645300   20 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    19138 Feb  8 18:47 written_2/travel_guides/berlitz1/IntroJapan.txt
202647304   12 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    10132 Feb  8 18:47 written_2/travel_guides/berlitz1/IntroJerusalem.txt
202647841   12 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    11857 Feb  8 18:47 written_2/travel_guides/berlitz1/IntroLakeDistrict.txt
202648107   12 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    11886 Feb  8 18:47 written_2/travel_guides/berlitz1/IntroLasVegas.txt
202648132    8 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23     6323 Feb  8 18:47 written_2/travel_guides/berlitz1/IntroLosAngeles.txt
202648713   12 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23     9927 Feb  8 18:47 written_2/travel_guides/berlitz1/IntroMadeira.txt
202649057   12 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    11562 Feb  8 18:47 written_2/travel_guides/berlitz1/IntroMadrid.txt
202649925   12 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23     8528 Feb  8 18:47 written_2/travel_guides/berlitz1/IntroMalaysia.txt
202649930   12 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23     9291 Feb  8 18:47 written_2/travel_guides/berlitz1/IntroMallorca.txt
202649934    8 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23     6818 Feb  8 18:47 written_2/travel_guides/berlitz1/JungleMalaysia.txt
202651519   28 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    20985 Feb  8 18:47 written_2/travel_guides/berlitz1/WhatToDublin.txt
202652143   28 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    21152 Feb  8 18:47 written_2/travel_guides/berlitz1/WhatToEdinburgh.txt
202652154   28 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    21659 Feb  8 18:47 written_2/travel_guides/berlitz1/WhatToEgypt.txt
202652239   32 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    26623 Feb  8 18:47 written_2/travel_guides/berlitz1/WhatToFWI.txt
202652243    4 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23     2324 Feb  8 18:47 written_2/travel_guides/berlitz1/WhatToFrance.txt
202652246   20 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    18503 Feb  8 18:47 written_2/travel_guides/berlitz1/WhatToGreek.txt
202652812    4 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23     2477 Feb  8 18:47 written_2/travel_guides/berlitz1/WhatToHawaii.txt
202655294   32 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    24756 Feb  8 18:47 written_2/travel_guides/berlitz1/WhatToHongKong.txt
202655364   44 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    38183 Feb  8 18:47 written_2/travel_guides/berlitz1/WhatToIbiza.txt
202656470   20 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    18898 Feb  8 18:47 written_2/travel_guides/berlitz1/WhatToIndia.txt
202656506   28 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    21343 Feb  8 18:47 written_2/travel_guides/berlitz1/WhatToIsrael.txt
202656561   32 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    26999 Feb  8 18:47 written_2/travel_guides/berlitz1/WhatToIstanbul.txt
202656596   28 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    22430 Feb  8 18:47 written_2/travel_guides/berlitz1/WhatToItaly.txt
202656632   92 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    86290 Feb  8 18:47 written_2/travel_guides/berlitz1/WhatToJamaica.txt
202657647   40 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    35438 Feb  8 18:47 written_2/travel_guides/berlitz1/WhatToJapan.txt
202657649   28 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    21180 Feb  8 18:47 written_2/travel_guides/berlitz1/WhatToLakeDistrict.txt
202657790   52 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    48170 Feb  8 18:47 written_2/travel_guides/berlitz1/WhatToLasVegas.txt
202658637   28 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    24076 Feb  8 18:47 written_2/travel_guides/berlitz1/WhatToLosAngeles.txt
202658650   32 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    28497 Feb  8 18:47 written_2/travel_guides/berlitz1/WhatToMadeira.txt
202658663   28 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    23497 Feb  8 18:47 written_2/travel_guides/berlitz1/WhatToMalaysia.txt
202658666   20 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    17417 Feb  8 18:47 written_2/travel_guides/berlitz1/WhatToMallorca.txt
202658668   92 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    87384 Feb  8 18:47 written_2/travel_guides/berlitz1/WhereToDublin.txt
202658684   84 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    79007 Feb  8 18:47 written_2/travel_guides/berlitz1/WhereToEdinburgh.txt
202658686   88 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    85505 Feb  8 18:47 written_2/travel_guides/berlitz1/WhereToEgypt.txt
202658883   68 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    64916 Feb  8 18:47 written_2/travel_guides/berlitz1/WhereToFWI.txt
202892698  256 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23   253959 Feb  8 18:47 written_2/travel_guides/berlitz1/WhereToFrance.txt
209329252   84 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    80111 Feb  8 18:47 written_2/travel_guides/berlitz1/WhereToGreek.txt
211154867    4 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23     2309 Feb  8 18:47 written_2/travel_guides/berlitz1/WhereToHawaii.txt
210187400   72 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    67601 Feb  8 18:47 written_2/travel_guides/berlitz1/WhereToHongKong.txt
210478709   48 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    42155 Feb  8 18:47 written_2/travel_guides/berlitz1/WhereToIbiza.txt
210478711  176 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23   172986 Feb  8 18:47 written_2/travel_guides/berlitz1/WhereToIndia.txt
210478712   88 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    84424 Feb  8 18:47 written_2/travel_guides/berlitz1/WhereToIsrael.txt
210478713   92 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    88932 Feb  8 18:47 written_2/travel_guides/berlitz1/WhereToIstanbul.txt
210478714  292 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23   294602 Feb  8 18:47 written_2/travel_guides/berlitz1/WhereToItaly.txt
210478722  192 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23   189061 Feb  8 18:47 written_2/travel_guides/berlitz1/WhereToJapan.txt
210716900   80 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    76530 Feb  8 18:47 written_2/travel_guides/berlitz1/WhereToJerusalem.txt
210716906   88 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    84671 Feb  8 18:47 written_2/travel_guides/berlitz1/WhereToLakeDistrict.txt
210716907   84 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    77840 Feb  8 18:47 written_2/travel_guides/berlitz1/WhereToLosAngeles.txt
210716909   68 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    65176 Feb  8 18:47 written_2/travel_guides/berlitz1/WhereToMadeira.txt
210716910   84 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    78028 Feb  8 18:47 written_2/travel_guides/berlitz1/WhereToMadrid.txt
210478708  184 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23   180940 Feb  8 18:47 written_2/travel_guides/berlitz1/WhereToMalaysia.txt
210716912   80 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    74270 Feb  8 18:47 written_2/travel_guides/berlitz1/WhereToMallorca.txt
210478710    8 drwxr-s---   2 cs15lwi23aun ieng6_cs15lwi23     8192 Feb  8 18:47 written_2/travel_guides/berlitz2
210716913   16 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    15389 Feb  8 18:47 written_2/travel_guides/berlitz2/Algarve-History.txt
210724002    8 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23     7996 Feb  8 18:47 written_2/travel_guides/berlitz2/Algarve-Intro.txt
210727897   16 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    16133 Feb  8 18:47 written_2/travel_guides/berlitz2/Algarve-WhatToDo.txt
210738877   72 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    69415 Feb  8 18:47 written_2/travel_guides/berlitz2/Algarve-WhereToGo.txt
210763340   16 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    15758 Feb  8 18:47 written_2/travel_guides/berlitz2/Amsterdam-History.txt
217201773   12 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23     8765 Feb  8 18:47 written_2/travel_guides/berlitz2/Amsterdam-Intro.txt
217201774   16 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    16133 Feb  8 18:47 written_2/travel_guides/berlitz2/Amsterdam-WhatToDo.txt
217201779   64 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    58911 Feb  8 18:47 written_2/travel_guides/berlitz2/Amsterdam-WhereToGo.txt
217201827   28 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    20481 Feb  8 18:47 written_2/travel_guides/berlitz2/Athens-History.txt
217201828   12 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23     8907 Feb  8 18:47 written_2/travel_guides/berlitz2/Athens-Intro.txt
217201829   20 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    17143 Feb  8 18:47 written_2/travel_guides/berlitz2/Athens-WhatToDo.txt
217201831   76 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    71349 Feb  8 18:47 written_2/travel_guides/berlitz2/Athens-WhereToGo.txt
217201832   20 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    16802 Feb  8 18:47 written_2/travel_guides/berlitz2/Bahamas-History.txt
217201833   12 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23     9107 Feb  8 18:47 written_2/travel_guides/berlitz2/Bahamas-Intro.txt
217201834   20 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    19719 Feb  8 18:47 written_2/travel_guides/berlitz2/Bahamas-WhatToDo.txt
217201835   76 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    73435 Feb  8 18:47 written_2/travel_guides/berlitz2/Bahamas-WhereToGo.txt
217201836   20 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    16431 Feb  8 18:47 written_2/travel_guides/berlitz2/Bali-History.txt
217201837   20 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    18112 Feb  8 18:47 written_2/travel_guides/berlitz2/Bali-WhatToDo.txt
217201838   84 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    78053 Feb  8 18:47 written_2/travel_guides/berlitz2/Bali-WhereToGo.txt
217201839   16 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    13127 Feb  8 18:47 written_2/travel_guides/berlitz2/Barcelona-History.txt
217201840   20 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    19052 Feb  8 18:47 written_2/travel_guides/berlitz2/Barcelona-WhatToDo.txt
217201841   76 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    72769 Feb  8 18:47 written_2/travel_guides/berlitz2/Barcelona-WhereToGo.txt
217201842   16 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    12702 Feb  8 18:47 written_2/travel_guides/berlitz2/Beijing-History.txt
217201843   28 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    21838 Feb  8 18:47 written_2/travel_guides/berlitz2/Beijing-WhatToDo.txt
217201844   68 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    63667 Feb  8 18:47 written_2/travel_guides/berlitz2/Beijing-WhereToGo.txt
217201845   28 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    22126 Feb  8 18:47 written_2/travel_guides/berlitz2/Berlin-History.txt
217201846   16 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    14688 Feb  8 18:47 written_2/travel_guides/berlitz2/Berlin-WhatToDo.txt
217201847   76 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    69890 Feb  8 18:47 written_2/travel_guides/berlitz2/Berlin-WhereToGo.txt
217201848   28 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    22386 Feb  8 18:47 written_2/travel_guides/berlitz2/Bermuda-WhatToDo.txt
217201849   64 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    60475 Feb  8 18:47 written_2/travel_guides/berlitz2/Bermuda-WhereToGo.txt
217201850   16 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    15046 Feb  8 18:47 written_2/travel_guides/berlitz2/Bermuda-history.txt
217201852   76 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    73074 Feb  8 18:47 written_2/travel_guides/berlitz2/Boston-WhereToGo.txt
217201854   16 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    12872 Feb  8 18:47 written_2/travel_guides/berlitz2/Budapest-History.txt
217201855   20 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    16916 Feb  8 18:47 written_2/travel_guides/berlitz2/Budapest-WhatToDo.txt
217201856   76 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    73535 Feb  8 18:47 written_2/travel_guides/berlitz2/Budapest-WhereoGo.txt
217201857   20 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    19139 Feb  8 18:47 written_2/travel_guides/berlitz2/California-History.txt
217201858   16 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    16255 Feb  8 18:47 written_2/travel_guides/berlitz2/California-WhatToDo.txt
217201859   76 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    73702 Feb  8 18:47 written_2/travel_guides/berlitz2/California-WhereToGo.txt
217201860   52 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    46093 Feb  8 18:47 written_2/travel_guides/berlitz2/Canada-History.txt
202637386  236 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23   235947 Feb  8 18:47 written_2/travel_guides/berlitz2/Canada-WhereToGo.txt
202637385   16 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    13919 Feb  8 18:47 written_2/travel_guides/berlitz2/CanaryIslands-History.txt
217201863   16 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    15587 Feb  8 18:47 written_2/travel_guides/berlitz2/CanaryIslands-WhatToDo.txt
217201864   80 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    76744 Feb  8 18:47 written_2/travel_guides/berlitz2/CanaryIslands-WhereToGo.txt
217201866   16 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    15364 Feb  8 18:47 written_2/travel_guides/berlitz2/Cancun-History.txt
217201867   20 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    18673 Feb  8 18:47 written_2/travel_guides/berlitz2/Cancun-WhatToDo.txt
217201868   72 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    66453 Feb  8 18:47 written_2/travel_guides/berlitz2/Cancun-WhereToGo.txt
217201853   36 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    29333 Feb  8 18:47 written_2/travel_guides/berlitz2/China-History.txt
217201869   16 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    12906 Feb  8 18:47 written_2/travel_guides/berlitz2/China-WhatToDo.txt
217201870  200 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23   198080 Feb  8 18:47 written_2/travel_guides/berlitz2/China-WhereToGo.txt
217201872   16 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    16143 Feb  8 18:47 written_2/travel_guides/berlitz2/Costa-History.txt
217201874   16 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    14889 Feb  8 18:47 written_2/travel_guides/berlitz2/Costa-WhatToDo.txt
217201875   76 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    73708 Feb  8 18:47 written_2/travel_guides/berlitz2/Costa-WhereToGo.txt
202637505   12 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    11981 Feb  8 18:47 written_2/travel_guides/berlitz2/CostaBlanca-History.txt
202637512   36 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    30453 Feb  8 18:47 written_2/travel_guides/berlitz2/CostaBlanca-WhatToDo.txt
202637495   16 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    15760 Feb  8 18:47 written_2/travel_guides/berlitz2/Crete-History.txt
217201879   20 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    16532 Feb  8 18:47 written_2/travel_guides/berlitz2/Crete-WhatToDo.txt
217201851   84 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    81548 Feb  8 18:47 written_2/travel_guides/berlitz2/Crete-WhereToGo.txt
217201880   52 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    48636 Feb  8 18:47 written_2/travel_guides/berlitz2/CstaBlanca-WhereToGo.txt
217201862   12 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    11789 Feb  8 18:47 written_2/travel_guides/berlitz2/Cuba-History.txt
217201918   20 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    17210 Feb  8 18:47 written_2/travel_guides/berlitz2/Cuba-WhatToDo.txt
217201865   80 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    76041 Feb  8 18:47 written_2/travel_guides/berlitz2/Cuba-WhereToGo.txt
217201985   20 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    18933 Feb  8 18:47 written_2/travel_guides/berlitz2/Nepal-History.txt
217201986   44 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    40450 Feb  8 18:47 written_2/travel_guides/berlitz2/Nepal-WhatToDo.txt
217201987   60 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    53280 Feb  8 18:47 written_2/travel_guides/berlitz2/Nepal-WhereToGo.txt
202655358   28 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    20746 Feb  8 18:47 written_2/travel_guides/berlitz2/NewOrleans-History.txt
217201873   16 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    13871 Feb  8 18:47 written_2/travel_guides/berlitz2/Paris-WhatToDo.txt
217283931   76 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    73204 Feb  8 18:47 written_2/travel_guides/berlitz2/Paris-WhereToGo.txt
217201876   20 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    20387 Feb  8 18:47 written_2/travel_guides/berlitz2/Poland-History.txt
217284541   20 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    19408 Feb  8 18:47 written_2/travel_guides/berlitz2/Poland-WhatToDo.txt
202645275   16 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    14604 Feb  8 18:47 written_2/travel_guides/berlitz2/Portugal-History.txt
217201830   20 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    17125 Feb  8 18:47 written_2/travel_guides/berlitz2/Portugal-WhatToDo.txt
217201861  124 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23   119651 Feb  8 18:47 written_2/travel_guides/berlitz2/Portugal-WhereToGo.txt
202637390   16 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    13736 Feb  8 18:47 written_2/travel_guides/berlitz2/PuertoRico-History.txt
202637498   28 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    20609 Feb  8 18:47 written_2/travel_guides/berlitz2/PuertoRico-WhatToDo.txt
217201984   72 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    66550 Feb  8 18:47 written_2/travel_guides/berlitz2/PuertoRico-WhereToGo.txt
217201989   16 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    14266 Feb  8 18:47 written_2/travel_guides/berlitz2/Vallarta-History.txt
217284893   40 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    36255 Feb  8 18:47 written_2/travel_guides/berlitz2/Vallarta-WhatToDo.txt
217285142   56 -rwxr-x---   1 cs15lwi23aun ieng6_cs15lwi23    52679 Feb  8 18:47 written_2/travel_guides/berlitz2/Vallarta-WhereToGo.txt
[cs15lwi23aun@ieng6-201]:skill-demo1-data:514$ 
```
In this example I am having the computer list out everything inside the written_2 directory, this can prove to be useful if you just want to see a big picture of everthing in a given directory.

## Command line command #4 `find [path] -type f -empty`
This command will go and check for any file that is empty and will return a list of the files that are empty and their respective file path.
This can prove to be useful when you want to check if something is taking up uneccesary space.

Example:
```
[cs15lwi23aun@ieng6-201]:skill-demo1-data:505$ cd written_2
[cs15lwi23aun@ieng6-201]:written_2:506$ touch "hello.txt"
[cs15lwi23aun@ieng6-201]:written_2:507$ touch "empty.txt"
[cs15lwi23aun@ieng6-201]:written_2:508$ cd ..                               
[cs15lwi23aun@ieng6-201]:skill-demo1-data:509$ find written_2 -type f -empty
written_2/hello.txt
written_2/empty.txt
```
In this example I am creating two empty files and placing them inside the written_2 directory and then going back out and finding the empty file.


To find these commands I found this website which had most of the commands : [Reference to Commands]([https://link-url-here.org](https://www.redhat.com/sysadmin/linux-find-command)) and I also looked at ``` man find``` for a list of commands and Chat GPT to have a better understanding of the commands .



