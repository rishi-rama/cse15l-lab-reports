# Lab Report 4
**4: ssh into ieng6**

Keys pressed:  `<up><enter>`
The command `ssh cs15lwi23aqn@ieng6.ucsd.edu` was 1 up in the search history, so I pressed the up arrow once to access it. Then I pressed enter to execute it
![image](https://user-images.githubusercontent.com/122561679/221721302-034f31f8-2c82-4b50-b4ae-857b4aec747c.png)


**5-9: Run tests and fix**

Keys pressed: `<up><up><enter>`


The command `git clone git@github.com:rishi-rama/lab7.git;cd lab7;javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar *.java;java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore ListExamplesTests;sed -i '43s/index1/index2/g' ListExamples.java;javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar *.java;java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore ListExamplesTests;git add ListExamples.java;git commit -m "fixed version";git push origin main` was 2 up in the search history, so I pressed up twice to access it then enter to run it.

This one command executes all the steps from 5-9 sequentially. It begins with cloning the forked git repository, then cd into the lab7 directory, then run the JUnit tests to show the failure, then use the sed command to edit line 43 and fix the failing code, then run the JUnit tests again to show they succeed, then commit and push the fixed code to Github

![image](https://user-images.githubusercontent.com/122561679/221721446-75de84b7-1193-4562-bee3-57f1d9071469.png)

