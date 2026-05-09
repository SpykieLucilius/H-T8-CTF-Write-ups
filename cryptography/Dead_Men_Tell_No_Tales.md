## Challenge Name: Dead Men Tell No Tales
**Category:** cryptography
**Points:** 499
**Solves:** 2

Challenge Description: 
In this challenge the description indicate that the language is hold but the cipher is even older. We are given a zip file containing a page with symbols on it. and the alphabet needed to translate it to roman characters. However, this is not enough to decode the message. We need to apply a Rot13 cipher to the alphabet to get the correct mapping of the letters.  

Artifact Files:
* [page.zip](./artifact/page.zip)

### Approach

**1. Finding the symbols**

To start the challenge i felt that it would be easier to do it manually since the text was not very long. I extracted the zip file and opened the page with the symbols. I then used the provided alphabet to translate the symbols into roman characters. However, the resulting text was still not readable.

**2. Applying the Rot13 cipher**

The hint in the description indicated that the cipher is even older than the hold language, which made me think of the Rot13 cipher. I applied the Rot13 cipher to the translated text and finally got the flag.

### Reflections
This challenge give clever hints in the description that helped me to find the solution. It was a nice exercise to practice decoding and applying ciphers. The challenge was not very difficult, but it was a good reminder to always pay attention to the hints provided in the description.

---
[Back to home](<../README.md>)