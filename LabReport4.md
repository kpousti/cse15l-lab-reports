
# Lab Report 4 

## Steps 4 - 9 from the lab 
---
# Step 4: 

First step we wanna complete is to `ssh` to gain remote access and then git clone the given respository.
- Keys pressed: `ssh` username@ieng6.ucsd.edu<enter>
- Effect: Initiates an SSH connection to the ieng6 server, allowing remote access.

 ![image](sshentry.pdf)


Due to my ssh key not being setup yet, I still do have to enter my password everytime.

# Step 5 
 
Using `<ctrl><r>` I was able to refernce my past history, primarily those commands made in the lab that allowed for a shortcut to be made. I then entered 'gi' in the reverse search and the clone with the selected repository showed up.
- Keys pressed: <ctrl><r>, gi<tab>
- Effect: Uses Ctrl+R to search the command history, then types "gi" and uses tab completion to select the git clone command for the repository.
- Keys pressed: <enter>
- Effect: Executes the git clone command and clones the repository to the local machine.

![Secnd](gitclone.pdf)

Once cloned, I pressed `<Enter>` and the ball was rollin...

![Third?](gitclone2.pdf)

After typing `ls` I could see lab 7/ listed. Then with past knowledge of how to do so, I changed the directory to lab 7 with the commmand;`cd l<tab>` This allowed for me to pratcice Profesors shortcut using `<Tab>`
- Keys pressed: ls
- Effect: Lists the contents of the current directory.
- Keys pressed: cd l<tab>
- Effect: Changes the directory to "lab 7" using tab completion.

# Step 6

Now proceeding to press `ls` we can see the contents of the file we then found a file Test.sh, I had to check what was in the bash script by typing `less te<tab>`

![four](lsoption.pdf)

Press `Q` in order to return back

now lets run the tests to see if it works 
typing in `bash te<tab>`

![five](2testsfailed.pdf)

When running `bash tesh.sh` we could see the 2 failed tests and which line the error is on.

# Step 7

We then go to the problematic file called ListExamples.java using the command `vim ListExamples.java` showing and allowing us acess to all the lines located in that file.

![six](javafile.pdf)

If you notice, we cannot edit and can only scroll up and down. We need to enter INSERT mode in vim, we can do this by pressing `I`

Now that we are in Insert mode,we can remember that the error is at line 44 as a editor we can choose to hit the key down to hold to attain the access point. We hold `<down>` key until we reach the error.

The goal is to for us the editors to read the underlying comment to change Index1 to Index2. We then listen and change this to help us fix error.

Make sure to exit INSERT mode by pressing `<Escape>` , we can then exit VIM by pressing `<Shift><;><W><Q>`.This allows us not to only quit from Vim but also save what we have changed.

 You can always check by typing `less ListExamples.java`

![seven](checktosee.pdf)
- Keys pressed: ls, less te<tab>
- Effect: Uses ls to list the contents of the current directory, then uses less to view the contents of the "Test.sh" file.
It showed up changed...

# Step 8

Running the test again,we press `bash test.sh` then `<enter>`, showing the fruit of our labor. 

![eight]passtest.pdf)
- Keys pressed: <up><up><up><up><enter>
- Effect: Uses the up arrow key to access the previous command from the command history. This retrieves the bash test.sh command from Step 6, allowing for easy re-execution of the test script.

![nine](passtest.pdf)

# Step 9

Our final step just needs us to commit the code to github.

![Ten](pushtogit.pdf)

The first thing we must do is type `git add .<enter>` in order add all the changed files. Then type in `git commit -m "fix"<enter>` to commit the changes, and finally type `git push<enter>` to push the changes.
- Keys pressed: <ctrl><r>, git push<enter>
- Effect: Initiates a reverse search using Ctrl-R. Searches for the git push command in the command history. Once found, executes the command to push the committed changes to the GitHub repository.b.

