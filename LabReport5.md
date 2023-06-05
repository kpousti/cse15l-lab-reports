# Lab Report 5, Debugging

For this lab we will be debugging and looking to fix an issue that arises on the code that we are presented with. 

---

# Part 1 

## Asking the questions to figuring out what the issue is with the code

The student submitted an issue they were having with their code. They gave the basic information to begin with, using Visual Studio code on a machine who ran MacOs. 

The issue their code was having was that it was not compiling correctly at all first. They created their own Bash script in order to run the JUnit script to call run the files and output it in a seperate text file to see what was the error. They also explained that the with any type of Test file he ran with the JUnit script it would always result in an error. 

With this being said, our bug will most likely be in the testing files and as well in the script so lets find out what the biggest issue was within the code


---

To start off we currently stand in the Student working directory of the code they were writing, this all consists in a folder that is the master folder. Now we are first running the bash script to see what the main issue is we

![one](StudentScreenShotOfTerminal1.png)
Based off what we were able to find in the terminal, the student called it using their command 
```
Bash tester.sh ArrayTests.java
```
Which in the terminal it seems like there is nothing wrong but then afterwards we are able to see that the real error consists in the text file output the student created from the bash script
![two](OutputPage1.png)

From this output messege it seemed like JUnit wasnt able to understand if the file they chose contianed any classes to which then the bug was on the users input, which was due to the way they entered the the file name. Since a Java file that contains a class that looks like it works correctly without any found errors first should compile correctly but this was not the case. Because of this I figured the bug was on the way they called the file they were trying to run, Pointing out that calling  `ArrayTests.java` was mostlikely not the correct way on how to call it. The student changed it and the bug was fixed 

![three](WorkFlowOfStudent.png)

Seeing that the files were able to compile correcty  and as well as the JUnit output file changing on their workflow showed that this was indeed the main bug that they were dealing with, so then all it took was to call their other testing files that they needed to see if they work well.

The second Testing file had some debugging issues as well. The student made an Array Filter algorithm where it when you gave the function an array of numbers, it would filter out numbers that were not prime.

![PrimeFilterBug](PrimeFilterBug.png)

Majority of the code was working well, when it cames to testing the edge cases of the code was when the code became a lot more buggy as shown in the problem the student brought up. Its interestint to see that one of the issues is the fact that we have reached the end of the code already.

We Call the code using the now fixed bash script by typing 
``` 
bash tester.sh MethodsTests
```
And we see from the JUnit output that there is an "End of Array" was actual, meaning that the code was expecting an empty array although the other two numbers were prime numbers.
![five](JunitOutput2.png)

After looking deeper in it, Its clearly shown that the bug is mainly in the condtional methods, If we tweek the by a bit we can get the optimal solution for this case. The way we can fix this is by splitting up `if(n == 1 || n % 2 == 0)` and moving it to what get prioritized first.

So instead of looking like this
![Split1](Split1.png)

We can interchange it like this
![Split2](Split2.png)

Which fixes our original problem because we are moving to when n soley equals 2 first, and when that condition isnt met it would move down to the next one which is finding if n has no remainders when dividing by 2 since that helps determine if a number is even or not. Prioritizing which steps the solver should use was incredibly important in order the understand each the larger error the code had.

And when running the bash script in the command line and looking at our out put in the other text file, we see that the bug is fixed
![last](BugFix2.png)

Now when the user throws any form of test to this method, it should always pass majority of the time.

For this scenario we Didn't really need to go out of the main directory from where we were in since for the most part everything worked well in the same working directory.

---

# Part 2 Reflection

I've been able to learn a lot about the shortcuts that can be quickly accesssed from my machine or almost any machine that I was able to learn and apply on a daily basis. We were able to apply these tools in the labs throughout the week that sometimes took a while but with the help of tutors it really made it a lot easier to learn and understand how it all worked. Personally I feel like these skills can be learned a lot more in depth from using them on software you can download online and seeing what else is capable from just the command line alone, I used to tamper around the command line and seeing which ever combination of words worked but now after this quarter I was able to learn and understand where it all came from to begin with which is something I do admire a lot and thank you for every tutor who tutored this quarter.
