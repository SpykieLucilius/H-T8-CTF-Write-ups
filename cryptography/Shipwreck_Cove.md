## Challenge Name: Shipwreck Cove
**Category:** cryptography
**Points:** 464
**Solves:** 7

Challenge Description: 
This challenge is about morse code. The file `lighthouse_log.txt` contains a log of a lighthouse, which includes some morse information. Our task is to decode the morse code to find the hidden flag.

Artifact Files:
* [lighthouse_log.txt](./artifact/lighthouse_log.txt)

### Approach

**1. Finding the morse code**

When we check the contents of `lighthouse_log.txt`, we can see that it contains a log of a lighthouse, which includes when the signal was send and for how long the light blinked. We can use this information to determine the morse code. A short blink (1s) represents a dot (.) and a long blink (3s) represents a dash (-). By analyzing the time log of each signal, we can also determine the separation between letters and words. A short separation (1s) represents a separation between letters, while a long separation (3s) represents a separation between words.

**2. Decoding the morse code**

After determining the morse code, we can decode it to find the hidden flag. We can use a morse code translator to convert the morse code into text. The decoded message will reveal the flag.


### Reflections
I did this challenge manually by analyzing the log and determining the morse code. It was a bit time-consuming. It would have been more efficient to write a script to automate the process of extracting the morse code from the log and decoding it. However, it was a fun exercise.

---
[Back to home](<../README.md>)