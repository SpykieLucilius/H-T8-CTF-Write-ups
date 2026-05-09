## Challenge Name: Python-as-a-Service 2/4
**Category:** Miscellaneous
**Points:** 25
**Solves:** 8

Challenge Description: 
This is the second part of the Python-as-a-Service challenge. In this part, we are given a netcat connection to a service running on a remote server. The service is a simple Python script that takes user input and executes it. Our goal is to find the second flag, which is located in a file named `flag2.txt`.

### Approach

**1. Use of `find` command**

To find the location of `flag2.txt`, we can use the `find` command to search for the file in the entire filesystem. The command to execute is:

```
__import__('os').system('find / -name "flag2.txt"').read()
```
This will return the path to the `flag2.txt` file, which is `/home/ctf/flag2.txt`. We can then read the contents of the flag file using:

```
__import__('os').system('cat /home/ctf/flag2.txt').read()
```


### Reflections
This challenge builds upon the first part by introducing the use of the `find` command to locate files on the filesystem. It demonstrates how we can leverage basic Linux commands to navigate and find specific files when we have limited information about their location.  

---
[Back to home](<../README.md>)