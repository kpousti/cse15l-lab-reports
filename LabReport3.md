# Lab Report 3


Out of the commands given, Ive chosen the `grep`command.


4 Interesting command line options involving `grep` that I've found include:


- `-i`
- `-r`
- `-n`
- `-c`



**i (ignore-case-search)**: Ignores case distinctions in patterns and input data
Match all lines that contain the word "  " in upper-case or lower-case.
- `-i` option is the one which you need to use

**r (recursive)**: When you want to search in all the files under the current directory and its sub directory. 
- `-r` option is the one which you need to use

**n (Search by String)**: The `n` option for grep is very useful when debugging files during compile errors. It displays the line number in the file of the given search string.
- `-n` option is the one which you need to use

**c (count)**: This option makes grep print all lines that do not match the pattern. It can be useful when you want to exclude certain lines from the output.
- `-c` option is the one which you need to use


## Examples of each command:
**i (ignore-case-search)**: Ignores case distinctions in patterns and input data**


### Example 1: Here is how you can call it on one of the files in the technical directory:
 ```
Command:grep -i "medical" stringsearch-data/technical/911report/chapter-1.txt
 ```

![image](firstt.pdf)

```
Command: grep -i "arrival" stringsearch-data/technical/911report/chapter-1.txt

```

![image](seccond.pdf)

## Example 2:
- **r (recursive)**: When you want to search in all the files under the current directory and its sub directory.
- This option enables grep to search for patterns recursively in subdirectories.

```
Command: stringsearch:336$ grep -r "instructions" stringsearch-data/technical/911report/chapter-1.txt
```

![image](tthird.pdf)
 
 
 ```
Command:stringsearch:337$ grep -r "General Wherley" stringsearch-data/technical/911report/chapter-1.txt
 ```

![image](fourrth.pdf)

### Example 3:
-**v (invert match)**
- This option makes grep print all lines that do not match the pattern. It can be useful when you want to exclude certain lines from the output.
```
Command: grep -n "gathered" stringsearch-data/technical/911report/chapter-1.txt

```

![image](5.pdf)

```
Command: grep -n "impoverished" stringsearch-data/technical/911report/chapter-1.txt
```

![image](six.pdf)
    
### Example 4:
- **c (count)**: This option makes grep print all lines that do not match the pattern. It can be useful when you want to exclude certain lines from the output.
- The `-c`option in grep makes it print only the count of matching lines rather than the matching lines themselves. This can be useful when you just want to know the number of lines that match a pattern.

```
Command: grep -c "earth" stringsearch-data/technical/911report/chapter-1.txt
```

![image](seven.pdf)

```
Command: grep -c "President" stringsearch-data/technical/911report/chapter-1.txt
```

![image](8.pdf)

## Resources I Used
(https://www.thegeekstuff.com/2009/03/15-practical-unix-grep-command-examples/)

(https://www.tecmint.com/12-practical-examples-of-linux-grep-command/)
