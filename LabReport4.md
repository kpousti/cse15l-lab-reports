
# Lab Report 4 

## Steps 4 - 9 from the lab 
---
# Step 4: 

First step we wanna complete is to `ssh` to gain remote access and then `git clone` the given respository.
- Keys pressed: `ssh` username@ieng6.ucsd.edu `<enter>`
- Effect: Initiates an SSH connection to the ieng6 server, allowing remote access.
- When prompted `<enter>` password 
- Due to my ssh key not being setup yet, I still do have to enter my password everytime.

 ![image](sshentry.pdf)


# Step 5 
 
Using `<ctrl><r>` I was able to reference my past history, primarily those commands made in the lab that allowed for this shortcut to be made. I then entered `gi` in the reverse search and the clone with the selected repository showed up.

To clone my forked repository from my GitHub account, I used the following keystrokes:

- Keys pressed: `<ctrl><r>` `gi<tab>` `<enter>`
- Keys pressed if no history: `git clone` `<enter>` "repository"
- Effect: Uses Ctrl+R to search the command history, types `gi,` and uses tab completion to select the` git clone` command for the repository. Then, executes the command to clone the repository to the local machine.


![Secnd](gitclone.pdf)

Once cloned, I pressed `<Enter>` and the ball was rollin...
- Keys pressed: `<Enter>`
- Effect: Executes the `git clone` command and clones the repository to the local machine.
![Third?](gitclone2.pdf)

After typing `ls` I could see lab 7/ listed. Then with past knowledge of how to do so, I changed the directory to lab 7 with the commmand;`cd l<tab>` this allowed for me to practice professors shortcut using `<tab>`
- Keys pressed: `ls``<enter>`
- Effect: Lists the contents of the current directory.
- Keys pressed: `cd l<tab>``<enter>`
- Effect: Changes the directory to "lab 7" using tab completion.
![four](lsoption.pdf)
# Step 6

After executing `ls`, I found a file named `test.sh`. To check the contents of the bash script using the `less` command, I used the following keystrokes:

- Keys pressed: `less te<tab>``<enter>`
- Effect: Uses the less command to view the contents of the `test.sh` file.
![four](testsh.pdf)


Pressing `Q` allowed me to return back.

To run the tests and observe the failures, I executed the following command:

- Keys pressed: `bash te<tab>``<enter>`
- Effect: Runs the tests by executing the `test.sh` bash script.

Running `bash tesh.sh` revealed the  failed tests and the line where the error occurs.

![five](2testsfailed.pdf)


# Step 7

We then go to the problematic file called `ListExamples.java` using the command `vim ListExamples.java` showing and allowing us access to all the lines located in that file.

To access the problematic file, `ListExamples.java` and edit it using the vim editor, I used the following keystrokes:

- Keys pressed: `vim ListExamples.java` `<enter>`
- Effect: Opens the `ListExamples.java` file in the vim editor, allowing access to all the lines in the file.
![six](javafile.pdf)

In the vim editor , I noticed that I could only scroll up and down and couldn't edit the file. To enter INSERT mode and make changes, I pressed `I`.

Now that I'm in Insert mode, I needed to locate the error at line 44. I pressed the `<down>` key to navigate down until I reached the error.

The goal was to read the underlying comment and change "Index1" to "Index2" to fix the error.

Once the changes were made, I exited INSERT mode by pressing `<Escape>`. To exit vim and save the changes, I used the keystrokes `<Shift><;><W><Q>`.


 You can always check by typing `less ListExamples.java`

![seven](checktosee.pdf)
- Keys pressed: `ls`, `less ListE<tab>``<enter>`
- Effect: Uses `ls` to list the contents of the current directory, then uses `less` to view the contents of the `ListExamples.java` file.
It showed up changed...

# Step 8

Running the test again,we press `bash test.sh` then `<enter>`, showing the fruit of our labor. 

- Keys pressed: `<up>``<up>``<up>``<up>``<enter>`
- Effect: Uses the up arrow key to access the previous command from the command history. This retrieves the `bash test.sh` command from Step 6, allowing for easy re-execution of the test script.

![nine](passtest.pdf)

# Step 9

The final step involves committing the code to GitHub. Here are the necessary keystrokes:

- Keys pressed:  `git push<enter>`
- Effect:  git pushes the changes to the GitHub repository using `git push`
 Once found, executes the command to push the committed changes to the GitHub repository.

![Ten](pushtogit.pdf)


