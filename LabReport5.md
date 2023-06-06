# Lab Report 5: Debugging

## Introduction
In this lab report, I will be addressing the debugging issue encountered in the provided code. The goal is to identify and fix the error to ensure the file runs without any issues.

# Part 1: Identifying the Issue


## Problem Description

The issue in the code is an ArrayIndexOutOfBoundsException error that occurs when accessing elements in the data array. The error message suggests that the index used to access the array is out of bounds.

### Environment (computer, operating system, web browser, terminal/editor, and so on)
- Mac Computer
- macOS
- Running on Terminal 
- Files built on Eclipse
- VS allowed bash to run



### Detail the symptom you're seeing. Be specific; include both what you're seeing and what you expected to see instead. Screenshots are great, and copy-pasted terminal output is also great. 

I'm working on a Java program that reads data from a file and performs calculations to find the average of the given file. However, I'm encountering an ArrayIndexOutOfBoundsException error, and I'm not sure what's causing it. It seems to happen when I'm accessing an element in an array. I'm expecting to see this program run and compute the average of numbers the given file. I suspect the issue lies in the loadData method, specifically when populating the data array.


![image](practice.pdf)

Any help in identifying and fixing the bug would be greatly appreciated. Thanks!


## Failure-Inducing Input and Context:


### Command to Compile the Java File:

`javac DataAnalyzer.java`

### Command to Run the Java Program:


`java DataAnalyzer`

![image](error1.pdf)

By following the steps mentioned above, including having the DataAnalyzer.java and data.txt files in the same directory, and running the commands `javac DataAnalyzer.java` and `java DataAnalyzer`, you will encounter the ArrayIndexOutOfBoundsException error due to a specific condition in the loadData method of the DataAnalyzer class.

The issue lies in the loop within the loadData method, which is responsible for populating the data array with values from the `data.txt` file.

![image](errorshown.pdf)

## Part 1.1: TA's Solution

### TA's Response
Hey there,

I've identified the issue in your code. It seems to be related to the loop in your loadData method. The problem lies in the loop condition `i <= size`, which should actually be `i < size`. This is because array indices start from 0 and go up to size - 1, so the loop should only iterate size times.

To fix the issue, please modify the loop condition as follows:

``
for (int i = 0; i < size; i++) {
    data[i] = scanner.nextDouble();
}
``
After making this change, recompile the DataAnalyzer.java file and run the program again. This should resolve the ArrayIndexOutOfBoundsException error you encountered.

If you have any further issues or need additional assistance, please let me know. 

I'm here to help!

---

# Part 1.2: Screenshot/Output after TA modification

Here's an updated screenshot showing the modified code:
![Image](errorcodefixed.pdf)
![Image](newnew.pdf)

After modifying the code as suggested, the program should run without any errors. The ArrayIndexOutOfBoundsException was occurring because the loop in the loadData method was going beyond the array bounds by using `i <= size` instead of `i < size`. By making this correction, we ensure that the loop only iterates through valid array indices.

# Setup:

---

## File & Directory Structure:
![image](newlibrary.pdf)

This is just my most recent library that was already under the Downloads folder on my mac making it very easy to access and run in terminal. This is my overall preference of running methods to see if they are working and correct. We as programmers can also do this so we get more adjusted to using different interfaces.

The Java file should be named `DataAnalyzer.java.`

The bash script file should be named `generate_data.sh.`

Both files should be located in the same directory. Which they are but one's in Visual Studio Code and one is in Eclipse.
## The contents of each file before fixing the bug:
![image](bash.pdf)

The `generate_data.sh` script uses shell commands to write the desired data into the `data.txt` file. This automation can be useful when you need to generate data files for testing or when you want to streamline the data generation process.

![image](codebefore.pdf)
### Full command line (or lines) to trigger the bug:

Compile the Java file:

``javac DataAnalyzer.java``

---
Run the Java program:

``java DataAnalyzer``

---

### Fixed code block:

``
for (int i = 0; i < size; i++) {
    data[i] = scanner.nextDouble();
}
``
### Commands Given:
![image](commandsgiven.pdf)

To fix the ArrayIndexOutOfBoundsException bug in the DataAnalyzer program, you need to modify the loop condition in the loadData method.

### What to edit to fix the bug:
In the original code, the loop condition `i <= size` allows the loop to iterate size + 1 times, which goes beyond the bounds of the data array. To correct this, you should change the loop condition to `i < size`, ensuring that the loop iterates exactly size times.

Here's the updated code that fixes the bug:

### DataAnalyzer.java:

```
import java.io.File;
import java.io.FileNotFoundException;
import java.util.Scanner;
    public static void main(String[] args) {
        loadData();
        analyzeData();
    }
 public static void loadData() {
        try {
            File file = new File(FILE_NAME);
            Scanner scanner = new Scanner(file);
            int size = scanner.nextInt();
            data = new double[size];
            for (int i = 0; i < size; i++) {
                data[i] = scanner.nextDouble();
            }
            scanner.close();
        } catch (FileNotFoundException e) {
            System.out.println("File not found: " + FILE_NAME);
        }
    }
     public static void analyzeData() {
        double sum = 0;
        for (int i = 0; i < data.length; i++) {
            sum += data[i];
        }
        double average = sum / data.length;
        System.out.println("Average: " + average);
    }

```


### generate_data.sh:

```

#!/bin/bash

echo "5" > data.txt
echo "10" >> data.txt
echo "20" >> data.txt
echo "30" >> data.txt
echo "40" >> data.txt
echo "50" >> data.txt

echo "Data file generated successfully."

```


This change ensures that the loop stays within the valid index range of the data array and prevents the ArrayIndexOutOfBoundsException error.

After making the necessary modifications, recompile the Java file and run the program again. The bug should be fixed, and the program should run without errors, correctly loading the data from the file.



## Part 2: 
During the second half of this quarter, I learned about the importance of proper error handling and debugging techniques. Through lab experiences, I gained a deeper understanding of how to identify and fix bugs in code, as well as the significance of handling exceptions effectively to ensure robustness and reliability in software development. This knowledge has greatly improved my problem-solving skills and allowed me to write more resilient code.
