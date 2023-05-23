# Lab Report 3


Out of the commands given Ive chosen the `grep`command.


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

**n (Search by String)**: The`n` option for grep is very useful when debugging files during compile errors. It displays the line number in the file of the given search string.
- `-n` option is the one which you need to use

**c (count)**: This option makes grep print all lines that do not match the pattern. It can be useful when you want to exclude certain lines from the output.
- `-c` option is the one which you need to use


## Examples of each command:
**i (ignore-case-search)**: Ignores case distinctions in patterns and input data**


### Example 1: Here is how you can call it on one of the files in the technical directory:
 ```
Command:grep -i "medical" stringsearch-data/technical/911report/chapter-1.txt
 ```
**Output**: At 8:41, Sweeney told Woodward that passengers in coach were under the impression that there was a routine medical emergency in first class. Other flight attendants were busy at duties such as getting medical supplies while Ong and Sweeney were reporting the events.

```
Command: grep -i "arrival" stringsearch-data/technical/911report/chapter-1.txt

```
**Output**: At the same time, the NEADS mission crew commander was dealing with the **arrival** of the Langley fighters over Washington, D.C., sorting out what their orders were with respect to potential targets. Shortly after 10:10, and having no knowledge either that United 93 had been heading toward Washington or that it had crashed, he explicitly instructed the Langley fighters: "negative- negative clearance to shoot" aircraft over the nation's capital.
    The Secret Service logged Mrs. Cheney's arrival at the White House at 9:52, and she joined her husband in the tunnel. According to contemporaneous notes, at 9:55 the Vice President was still on the phone with the President advising that three planes were missing and one had hit the Pentagon. We believe this is the same call in which the Vice President urged the President not to return to Washington. After the call ended, Mrs. Cheney and the Vice President moved from the tunnel to the shelter conference room.
    The Vice President remembered placing a call to the President just after entering the shelter conference room. There is conflicting evidence about when the Vice President arrived in the shelter conference room. We have concluded, from the available evidence, that the Vice President arrived in the room shortly before 10:00, perhaps at 9:58. The Vice President recalled being told, just after his **arrival**, that the Air Force was trying to establish a combat air patrol over Washington.

## Example 2:
- **r (recursive)**: When you want to search in all the files under the current directory and its sub directory.
- This option enables grep to search for patterns recursively in subdirectories.

```
Command: stringsearch:336$ grep -r "instructions" stringsearch-data/technical/911report/chapter-1.txt
```
**Output**:  At that same time, American 11 had its last routine communication with the ground when it acknowledged navigational instructions from the FAA's air traffic control (ATC) center in Boston. Sixteen seconds after that transmission, ATC instructed the aircraft's pilots to climb to 35,000 feet. That message and all subsequent attempts to contact the flight were not acknowledged. From this and other evidence, we believe the hijacking began at 8:14 or shortly thereafter.
    The Vice President stated that he called the President to discuss the rules of engagement for the CAP. He recalled feeling that it did no good to establish the CAP unless the pilots had instructions on whether they were authorized to shoot if the plane would not divert. He said the President signed off on that concept. The President said he remembered such a conversation, and that it reminded him of when he had been an interceptor pilot. The President emphasized to us that he had authorized the shootdown of hijacked aircraft.
    At 10:39, the Vice President updated the Secretary on the air threat conference: Vice President: There's been at least three instances here where we've had reports of aircraft approaching Washington-a couple were confirmed hijack. And, pursuant to the President's instructions I gave authorization for them to be taken out. Hello?
    SecDef: So we've got a couple of aircraft up there that have those instructions at this present time?
    General David Wherley-the commander of the 113th Wing-reached out to the Secret Service after hearing secondhand reports that it wanted fighters airborne. A Secret Service agent had a phone in each ear, one connected to Wherley and the other to a fellow agent at the White House, relaying instructions that the White House agent said he was getting from the Vice President. The guidance for Wherley was to send up the aircraft, with orders to protect the White House and take out any aircraft that threatened the Capitol. General Wherley translated this in military terms to flying "weapons free"-that is, the decision to shoot rests in the cockpit, or in this case in the cockpit of the lead pilot. He passed these instructions to the pilots that launched at 10:42 and afterward.
 
 
 ```
Command:stringsearch:337$ grep -r "General Wherley" stringsearch-data/technical/911report/chapter-1.txt
 ```
**Output**: General David Wherley-the commander of the 113th Wing-reached out to the Secret Service after hearing secondhand reports that it wanted fighters airborne. A Secret Service agent had a phone in each ear, one connected to Wherley and the other to a fellow agent at the White House, relaying instructions that the White House agent said he was getting from the Vice President. The guidance for Wherley was to send up the aircraft, with orders to protect the White House and take out any aircraft that threatened the Capitol. General Wherley translated this in military terms to flying "weapons free"-that is, the decision to shoot rests in the cockpit, or in this case in the cockpit of the lead pilot. He passed these instructions to the pilots that launched at 10:42 and afterward.

### Exmaple 3:
-**v (invert match)**
- This option makes grep print all lines that do not match the pattern. It can be useful when you want to exclude certain lines from the output.
```
Command: grep -n "gathered" stringsearch-data/technical/911report/chapter-1.txt

```
**Output**: 728 He was, and is, right. But the conflict did not begin on 9/11. It had been publicly declared years earlier, most notably in a declaration faxed early in 1998 to an Arabic-language newspaper in London. Few Americans had noticed it. The fax had been sent from thousands of miles away by the followers of a Saudi exile gathered in one of the most remote and impoverished countries on earth.
```
Command: grep -n "impoverished" stringsearch-data/technical/911report/chapter-1.txt
 ```
**Output**: 728: He was, and is, right. But the conflict did not begin on 9/11. It had been publicly declared years earlier, most notably in a declaration faxed early in 1998 to an Arabic-language newspaper in London. Few Americans had noticed it. The fax had been sent from thousands of miles away by the followers of a Saudi exile gathered in one of the most remote and impoverished countries on earth.
    
### Example 4:
- **c (count)**: This option makes grep print all lines that do not match the pattern. It can be useful when you want to exclude certain lines from the output.
- The `-c`option in grep makes it print only the count of matching lines rather than the matching lines themselves. This can be useful when you just want to know the number of lines that match a pattern.
```
Command:[cs15lsp23ms@ieng6-202]:stringsearch:351$ grep -c "earth" stringsearch-data/technical/911report/chapter-1.txt
```

### Output:1
```

Command: stringsearch:351$ grep -c "President" stringsearch-data/technical/911report/chapter-1.txt
```
### Output: 6
## Resources I Used:
(https://www.thegeekstuff.com/2009/03/15-practical-unix-grep-command-examples/)

(https://www.tecmint.com/12-practical-examples-of-linux-grep-command/)
