Lab Report 3
Out of the commands given ive chosen the grep command.
4 Interesting command line options involving grep that ive found include:





-**i**<br>
-**r**<br>
-**v**<br>
-**c**<br>
This option makes grep ignore case distinctions while searching for patterns. It can be useful when you want to search for a pattern but are not sure about its exact case.
**r (recursive)** <br>
This option enables grep to search for patterns recursively in subdirectories.
**v** (invert match)** <br>
This option makes grep print all lines that do not match the pattern. It can be useful when you want to exclude certain lines from the output.
**c (count)** <br>
This option makes grep print only the amount of lines that have that word.

Examples of each command:
**i**
Example 1: Here is how you can call it on one of the files in the technical directory:
 
Command:grep -i "medical" stringsearch-data/technical/911report/chapter-1.txt
 
  Output:At 8:41, Sweeney told Woodward that passengers in coach were under the impression that there was a routine medical emergency in first class. Other flight attendants were busy at duties such as getting medical supplies while Ong and Sweeney were reporting the events.


Command: stringsearch:330$ grep -i "shoot" stringsearch-data/technical/911report/chapter-1.txt

Output: Prior to 9/11, it was understood that an order to shoot down a commercial aircraft would have to be issued by the National Command Authority (a phrase used to describe the president and secretary of defense). Exercise planners also assumed that the aircraft would originate from outside the United States, allowing time to identify the target and scramble interceptors. The threat of terrorists hijacking commercial airliners within the United States-and using them as guided missiles-was not recognized by NORAD before 9/11. Notwithstanding the identification of these emerging threats, by 9/11 there were only seven alert sites left in the United States, each with two fighter aircraft on alert. This led some NORAD commanders to worry that NORAD was not postured adequately to protect the United States.
    At the same time, the NEADS mission crew commander was dealing with the arrival of the Langley fighters over Washington, D.C., sorting out what their orders were with respect to potential targets. Shortly after 10:10, and having no knowledge either that United 93 had been heading toward Washington or that it had crashed, he explicitly instructed the Langley fighters: "negative- negative clearance to shoot" aircraft over the nation's capital.
    At 10:03, the conference received reports of more missing aircraft, "2 possibly 3 aloft," and learned of a combat air patrol over Washington. There was discussion of the need for rules of engagement. Clarke reported that they were asking the President for authority to shoot down aircraft. Confirmation of that authority came at 10:25, but the commands were already being conveyed in more direct contacts with the Pentagon.
    United 93 and the Shootdown Order On the morning of 9/11, the President and Vice President stayed in contact not by an open line of communication but through a series of calls. The President told us he was frustrated with the poor communications that morning. He could not reach key officials, including Secretary Rumsfeld, for a period of time. The line to the White House shelter conference room-and the Vice President- kept cutting off.
    The Vice President stated that he called the President to discuss the rules of engagement for the CAP. He recalled feeling that it did no good to establish the CAP unless the pilots had instructions on whether they were authorized to shoot if the plane would not divert. He said the President signed off on that concept. The President said he remembered such a conversation, and that it reminded him of when he had been an interceptor pilot. The President emphasized to us that he had authorized the shootdown of hijacked aircraft.
    The Vice President was logged calling the President at 10:18 for a twominute conversation that obtained the confirmation. On Air Force One, the President's press secretary was taking notes; Ari Fleischer recorded that at 10:20, the President told him that he had authorized a shootdown of aircraft if necessary.
    The commander of NORAD, General Ralph Eberhart, was en route to the NORAD operations center in Cheyenne Mountain, Colorado, when the shootdown order was communicated on the air threat conference call. He told us that by the time he arrived, the order had already been passed down NORAD's chain of command.
    It is not clear how the shootdown order was communicated within NORAD. But we know that at 10:31, General Larry Arnold instructed his staff to broadcast the following over a NORAD instant messaging system: "10:31 Vice president has cleared to us to intercept tracks of interest and shoot them down if they do not respond per [General Arnold]."
    In upstate New York, NEADS personnel first learned of the shootdown order from this message: Floor Leadership: You need to read this. . . . The Region Commander has declared that we can shoot down aircraft that do not respond to our direction. Copy that?
    Controllers: Right now no, but- Floor Leadership: Okay? Okay, you read that from the Vice President, right? Vice President has cleared. Vice President has cleared us to intercept traffic and shoot them down if they do not respond per [General Arnold]. In interviews with us, NEADS personnel expressed considerable confusion over the nature and effect of the order.
    In most cases, the chain of command authorizing the use of force runs from the president to the secretary of defense and from the secretary to the combatant commander. The President apparently spoke to Secretary Rumsfeld for the first time that morning shortly after 10:00. No one can recall the content of this conversation, but it was a brief call in which the subject of shootdown authority was not discussed.
    As this exchange shows, Secretary Rumsfeld was not in the NMCC when the shootdown order was first conveyed. He went from the parking lot to his office (where he spoke to the President), then to the Executive Support Center, where he participated in the White House video teleconference. He moved to the NMCC shortly before 10:30, in order to join Vice Chairman Myers. Secretary Rumsfeld told us he was just gaining situational awareness when he spoke with the Vice President at 10:39. His primary concern was ensuring that the pilots had a clear understanding of their rules of engagement.
    The Vice President was mistaken in his belief that shootdown authorization had been passed to the pilots flying at NORAD's direction. By 10:45 there was, however, another set of fighters circling Washington that had entirely different rules of engagement. These fighters, part of the 113th Wing of the District of Columbia Air National Guard, launched out of Andrews Air Force Base in Maryland in response to information passed to them by the Secret Service. The first of the Andrews fighters was airborne at 10:38.
    General David Wherley-the commander of the 113th Wing-reached out to the Secret Service after hearing secondhand reports that it wanted fighters airborne. A Secret Service agent had a phone in each ear, one connected to Wherley and the other to a fellow agent at the White House, relaying instructions that the White House agent said he was getting from the Vice President. The guidance for Wherley was to send up the aircraft, with orders to protect the White House and take out any aircraft that threatened the Capitol. General Wherley translated this in military terms to flying "weapons free"-that is, the decision to shoot rests in the cockpit, or in this case in the cockpit of the lead pilot. He passed these instructions to the pilots that launched at 10:42 and afterward.
    Had it not crashed in Pennsylvania at 10:03, we estimate that United 93 could not have reached Washington any earlier than 10:13, and probably would have arrived before 10:23. There was only one set of fighters circling Washington during that time frame-the Langley F-16s. They were armed and under NORAD's control. After NEADS learned of the hijacking at 10:07, NORAD would have had from 6 to 16 minutes to locate the flight, receive authorization to shoot it down, and communicate the order to the pilots, who (in the same span) would have had to authenticate the order, intercept the flight, and execute the order.
    At that point in time, the Langley pilots did not know the threat they were facing, did not know where United 93 was located, and did not have shootdown authorization.
    Third, NEADS needed orders to pass to the pilots. At 10:10, the pilots over Washington were emphatically told, "negative clearance to shoot." Shootdown authority was first communicated to NEADS at 10:31. It is possible that NORAD commanders would have ordered a shootdown in the absence of the authorization communicated by the Vice President, but given the gravity of the decision to shoot down a commercial airliner, and NORAD's caution that a mistake not be made, we view this possibility as unlikely.

Source: Linuxize - grep Command in Linux with Examples
 The Geek Stuff - 12 Practical Examples of Linux grep Command
Example 2:
-r (recursive)
This option enables grep to search for patterns recursively in subdirectories.


Command: stringsearch:336$ grep -r "instructions" stringsearch-data/technical/911report/chapter-1.txt

Output:  At that same time, American 11 had its last routine communication with the ground when it acknowledged navigational instructions from the FAA's air traffic control (ATC) center in Boston. Sixteen seconds after that transmission, ATC instructed the aircraft's pilots to climb to 35,000 feet. That message and all subsequent attempts to contact the flight were not acknowledged. From this and other evidence, we believe the hijacking began at 8:14 or shortly thereafter.
    The Vice President stated that he called the President to discuss the rules of engagement for the CAP. He recalled feeling that it did no good to establish the CAP unless the pilots had instructions on whether they were authorized to shoot if the plane would not divert. He said the President signed off on that concept. The President said he remembered such a conversation, and that it reminded him of when he had been an interceptor pilot. The President emphasized to us that he had authorized the shootdown of hijacked aircraft.
    At 10:39, the Vice President updated the Secretary on the air threat conference: Vice President: There's been at least three instances here where we've had reports of aircraft approaching Washington-a couple were confirmed hijack. And, pursuant to the President's instructions I gave authorization for them to be taken out. Hello?
    SecDef: So we've got a couple of aircraft up there that have those instructions at this present time?
    General David Wherley-the commander of the 113th Wing-reached out to the Secret Service after hearing secondhand reports that it wanted fighters airborne. A Secret Service agent had a phone in each ear, one connected to Wherley and the other to a fellow agent at the White House, relaying instructions that the White House agent said he was getting from the Vice President. The guidance for Wherley was to send up the aircraft, with orders to protect the White House and take out any aircraft that threatened the Capitol. General Wherley translated this in military terms to flying "weapons free"-that is, the decision to shoot rests in the cockpit, or in this case in the cockpit of the lead pilot. He passed these instructions to the pilots that launched at 10:42 and afterward.
 
 
 
Command:stringsearch:337$ grep -r "General Wherley" stringsearch-data/technical/911report/chapter-1.txt
 
Output:General David Wherley-the commander of the 113th Wing-reached out to the Secret Service after hearing secondhand reports that it wanted fighters airborne. A Secret Service agent had a phone in each ear, one connected to Wherley and the other to a fellow agent at the White House, relaying instructions that the White House agent said he was getting from the Vice President. The guidance for Wherley was to send up the aircraft, with orders to protect the White House and take out any aircraft that threatened the Capitol. General Wherley translated this in military terms to flying "weapons free"-that is, the decision to shoot rests in the cockpit, or in this case in the cockpit of the lead pilot. He passed these instructions to the pilots that launched at 10:42 and afterward.

Exmaple 3:
-v (invert match)
This option makes grep print all lines that do not match the pattern. It can be useful when you want to exclude certain lines from the output.

Command: grep -v "bythe" stringsearch-data/technical/911report/chapter-1.txt

Output:  First, the Langley pilots were never briefed about the reason they were scrambled. As the lead pilot explained, "I reverted to the Russian threat. . . . I'm thinking cruise missile threat from the sea. You know you look down and see the Pentagon burning and I thought the bastards snuck one by us. . . . [Y]ou couldn't see any airplanes, and no one told us anything." The pilots knew their mission was to divert aircraft, but did not know that the threat came from hijacked airliners

Command: grep -v "bythe" stringsearch-data/technical/911report/chapter-1.txt
 
 Output:First, the Langley pilots were never briefed about the reason they were scrambled. As the lead pilot explained, "I reverted to the Russian threat. . . . I'm thinking cruise missile threat from the sea. You know you look down and see the Pentagon burning and I thought the bastards snuck one by us. . . . [Y]ou couldn't see any airplanes, and no one told us anything." The pilots knew their mission was to divert aircraft, but did not know that the threat came from hijacked airliners
    
Example 4:
the -c option in grep makes it print only the count of matching lines rather than the matching lines themselves. This can be useful when you just want to know the number of lines that match a pattern.

Command:[cs15lsp23ms@ieng6-202]:stringsearch:351$ grep -c "earth" stringsearch-data/technical/911report/chapter-1.txt


Output:1


Command: stringsearch:351$ grep -c "President" stringsearch-data/technical/911report/chapter-1.txt

Output: 6
