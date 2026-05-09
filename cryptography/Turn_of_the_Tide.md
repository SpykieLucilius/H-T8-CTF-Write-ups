## Challenge Name: Turn of the Tide
**Category:** cryptography
**Points:** 311
**Solves:** 12

Challenge Description: 
In this challenge, we are given a text file named `challenge.txt` that contains a message encoded using base64. Our task is to decode the message to reveal the hidden flag.

Artifact Files:
* [challenge.txt](./artifact/challenge.txt)

### Approach

**1. Decode and reverse the base64 encoded message**

When checking the contents of `challenge.txt`, we can see that it is a base64 encoded string. We can use a simple command to decode it:

```
cat challenge.txt | base64 -d
```
Looking at the decoded message, we can see that it is reversed. So we need to reverse the string to get the correct message. We can do this using the `rev` command:

```
cat challenge.txt | base64 -d | rev
```

### Reflections
A simple base64 decoding challenge with a twist of reversing the string. It was a good exercise to practice basic command-line tools for decoding and manipulating strings. The challenge was straightforward.

---
[Back to home](../README.md)