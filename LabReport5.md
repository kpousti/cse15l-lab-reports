# Lab Report 5, Debugging

For this lab we will be debugging and looking to fix an issue that arises on the code that we are presented with. 

---

# Part 1 

## Asking the questions to figuring out what the issue is with the code



# Part 2: 
## A response from a TA asking a leading question or suggesting a command to try 
---
Response from TA

Hey there,

It looks like the issue might be related to the loop in your loadData method. The loop condition i <= size should be changed to i < size because array indices start from 0 and go up to size - 1.

Could you try modifying the loop condition and run the program again? Let me know if it resolves the issue or if you encounter any other errors.
You can update the loop condition as follows:

``
for (int i = 0; i < size; i++) {
    data[i] = scanner.nextDouble();
}
``
Give it a try and let me know if it resolves the ArrayIndexOutOfBoundsException error. Feel free to share any terminal output or screenshots of the result.

---
# Part 3:
Screenshot/Output after modification

Here's an updated screenshot showing the modified code:
## Setup
After modifying the code as suggested, the program should run without any errors. The ArrayIndexOutOfBoundsException was occurring because the loop in the loadData method was going beyond the array bounds by using i <= size instead of i < size. By making this correction, we ensure that the loop only iterates through valid array indices.

Setup Information:

File & Directory Structure:

File & Directory Structure:

The Java file should be named `DataAnalyzer.java.`
The bash script file should be named `generate_data.sh.`
Both files should be located in the same directory.

## DataAnalyzer.java:
``
import java.io.File;
import java.io.FileNotFoundException;
import java.util.Scanner;

public class DataAnalyzer {
    private static final String FILE_NAME = "data.txt";
    private static double[] data;

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
            for (int i = 0; i <= size; i++) {
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
}
``

generate_data.sh:
bash
Copy code
``
#!/bin/bash

echo "5" > data.txt
echo "10.5" >> data.txt
echo "7.2" >> data.txt
echo "3.8" >> data.txt
echo "9.1" >> data.txt
echo "6.4" >> data.txt

echo "Data file generated successfully."

``

Full command line (or lines) to trigger the bug:

Compile the Java file:
Copy code
``javac DataAnalyzer.java``
Run the Java program:
Copy code
``java DataAnalyzer``
Description of what to edit to fix the bug:
In the loadData method of the DataAnalyzer.java file, modify the loop condition in the for loop as follows:

java
Copy code
``
for (int i = 0; i < size; i++) {
    data[i] = scanner.nextDouble();
}
``
This change ensures that the loop stays within the valid index range of the data array and prevents the ArrayIndexOutOfBoundsException error.

After making the necessary modifications, recompile the Java file and run the program again. The bug should be fixed, and the program should run without errors, correctly loading the data from the file.

Let me know if you need any further assistance!
