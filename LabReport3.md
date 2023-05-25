# Lab Report 3


Out of the commands given, Ive chosen the `grep`command.


4 Interesting command line options involving `grep` that I've found include:


- `-i`
- `-r`
- `-n`
- `-c`



**i (ignore-case-search)**:  Ignores case distinctions in patterns and input data. Matches all lines that contain the specified word, regardless of the case.
- `-i` option is the one which you need to use

**r (recursive)**: Performs a recursive search in all the files under the current directory and its subdirectories.
- `-r` option is the one which you need to use

**n (Search by String)**: The `n` option for grep is very useful when debugging files during compile errors. Displays the line number in the file of the given search string.
- `-n` option is the one which you need to use

**c (count)**: This option makes grep print all lines that do not match the pattern. It can be useful when you want to exclude certain lines from the output. Prints the count of lines that do not match the pattern.
- `-c` option is the one which you need to use


## Examples of each command:
**i (ignore-case-search)**: Ignores case distinctions in patterns and input data
- This is useful when you want to search through a file and want to match all lines containing the input given, especially special becuase it is case insentive looking for all types.
- This can be a editors best friend as he can find all instances of a mistyped word or sequence without having to change capitalization

## Example 1: Here is how you can call it on one of the files in the given directory
 ```
Command: grep -i "medical" stringsearch-data/technical/911report/chapter-1.txt
 ```

![image](firstt.pdf)

```
Command: grep -i "arrival" stringsearch-data/technical/911report/chapter-1.txt
```
![image](seccond.pdf)


## Example 2:
- **r (recursive)**: When you want to search in all the files under the current directory and its sub directory.
- This option enables grep to search for patterns recursively in subdirectories.
- This is a "Deeper" search than `-i` as it searchs for all of the given input in the directories and sub directorys. The biggest difference is the case sensitivity that this hold compared to command `-i`

```
Command: stringsearch:336$ grep -r "instructions" stringsearch-data/technical/911report/chapter-1.txt
```
![image](tthird.pdf)
 
  ```
Command: stringsearch:337$ grep -r "General Wherley" stringsearch-data/technical/911report/chapter-1.txt
 ```

![image](fourrth.pdf)


## Example 3:
- **n (Search by String)**: The `n` option for grep is very useful when debugging files during compile errors. It displays the line number in the file of the given search string.
- This is very valuable when looking for certain lines where a variable is present. This allows editors to find known errors and the output to show the given line with line number. This is shown here but both of these words are on the same line 728.
```
Command: grep -n "gathered" stringsearch-data/technical/911report/chapter-1.txt
```

![image](5.pdf)

```
Command: grep -n "impoverished" stringsearch-data/technical/911report/chapter-1.txt
```

![image](six.pdf)


## Example 4:
- **c (count)**: This option makes grep print all lines that do not match the pattern. It can be useful when you want to exclude certain lines from the output.
- The `-c`option in grep makes it print only the count of matching lines rather than the matching lines themselves. This can be useful when you just want to know the number of lines that match a pattern.
- This can allow the editor or viewer to see the amount of lines surrounding the assocated input and see how/if there is context surrounding it.

```
Command: grep -c "earth" stringsearch-data/technical/911report/chapter-1.txt
```

![image](seven.pdf)

```
Command: grep -c "President" stringsearch-data/technical/911report/chapter-1.txt 
```

![image](8.pdf)
---
## Resources I Used

- [Overall Scope](https://www.thegeekstuff.com/2009/03/15-practical-unix-grep-command-examples/)

- [Specific Commands](https://www.tecmint.com/12-practical-examples-of-linux-grep-command/)

- [More Commands](https://www.digitalocean.com/community/tutorials/grep-command-in-linux-unix)

- [Even More Commands](https://www.freecodecamp.org/news/grep-command-in-linux-usage-options-and-syntax-examples/)
