## Challenge Name: Python-as-a-Service 1/4
**Category:** Miscellaneous
**Points:** 25
**Solves:** 14

**Challenge Description:**
In this challenge, we are given a netcat connection to a service running on a remote server. The service is a simple Python script that takes user input and executes it.

### Approach

**1. Python "eval" vulnerability**

The service is vulnerable to a Python "eval" vulnerability, which allows us to execute arbitrary Python code on the server. We can use this vulnerability to read the contents of the flag file.

The line to inject our payload is:
```
__import__('os').system('WRITE COMMAND HERE').read()
```
To find the flag, we can use the following command:
```
__import__('os').system('ls -la').read()
```

This will display the contents of the current directory, which includes a file named `flag1.txt`. We can then read the flag file using:
```
__import__('os').system('cat flag1.txt').read()
```

### Reflections

This challenge serve as good introduction to the eval vulnerability in Python. It is basic but an effective way to demonstrate how user input can be exploited if not properly sanitized.
  

---
[Back to home](<../README.md>)