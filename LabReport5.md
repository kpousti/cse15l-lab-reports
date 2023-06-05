# Lab Report 5, Debugging

For this lab we will be debugging and looking to fix an issue that arises on the code that we are presented with. 

---

# Part 1 

## Asking the questions to figuring out what the issue is with the code



# Part 2: A response from a TA asking a leading question or suggesting a command to try 
---
Hey there,

It seems like the issue might be caused by an off-by-one error in the loop condition when populating the data array. In your loadData method, try modifying the loop condition from i <= size to i < size to ensure the loop stays within the bounds of the array indices.

You can update the loop condition as follows:

``
for (int i = 0; i < size; i++) {
    data[i] = scanner.nextDouble();
}
``
Give it a try and let me know if it resolves the ArrayIndexOutOfBoundsException error. Feel free to share any terminal output or screenshots of the result.
---
