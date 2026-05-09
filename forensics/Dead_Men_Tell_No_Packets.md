## Challenge Name: Dead Men Tell No Packets
**Category:** forensics
**Points:** 475
**Solves:** 6

Challenge Description: 
In this challenge we need to analyze a pcap file and find the hidden flag. The pcap file contains network traffic captures, and we need to analyze it to find the flag.

Artifact Files:
* [dead_men_tell_no_packets.pcap](./artifact/dead_men_tell_no_packets.pcap)

### Approach

**1. Analyze the pcap file**

By going through the pcap file using Wireshark, I noticed that some plaintext data was being transmitted over the network. It displayed some conversation between pirates, worried about the intern mistake in protecting the secrets. It mentioned that part of the pass was hidden in mail exchanges and dns queries. It also gave the last part of the pass in Base64 encoding. I decoded the Base64 string.

**2. Finding the other part of the pass**

Since the last part started with `part3`, I guessed that the other part of the pass would be `part1` and `part2`. I looked for any plaintext data in the pcap file that contained these strings. I easily found those pass like this.

**3. Combine the parts of the pass and unlocking the zip file**

The message exchange mentioned a chest. I also found that a zip file hinting to be the chest was being transmitted over the network. I downloaded the zip file and tried to open it. It was protected by a password, so I combined the three parts of the pass that I found in the pcap file and used it to unlock the zip file. Inside the zip file, I found a text file that contained the flag.


### Reflections
I love wireshark challenges, they are always fun to analyze and find the hidden secrets in the network traffic. This challenge in multiple steps was fun to solve. It's also nice that "lazy" methodes like searching for plaintext data in the pcap file can be very effective in finding the flag.  

---
[Back to home](<../README.md>)