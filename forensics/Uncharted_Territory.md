## Challenge Name: Uncharted Territory
**Category:** forensics
**Points:** 419
**Solves:** 10

Challenge Description: 
In this challenge we're given a zip file that contains a lot of subdirectories with the same files each time. We need to analyze the files and find the right directory that contains the flag.

Artifact Files:
* [territory.zip](./artifact/territory.zip)

### Approach

**1. Spot the right directory**

To find the correct directory, I tought that the folder containing the flag would obviously be heavier that the others. So I used the `ls -lh` command to check the size of each directory and find the one that is heavier than the others. Once I found the right directory, I checked its contents and found the flag printed in a picture of a pirate cat.


### Reflections
This was a fun challenge to come up with a solution to find the right directory. It was a good reminder that sometimes the solution to a challenge can be as simple as checking the size of the files.
  
---
[Back to home](<../README.md>)