## Challenge Name: Sanity Check
**Category:** Welcome
**Points:** 475
**Solves:** 6

Challenge Description: 
This one is a bit of a trick challenge. The flag is well hidden within a message in the server. It's written in invisible unicode characters, so you won't see it until you realize there's extra characters in the message.

### Approach

**1. Analyzing the hidden message**

With hints indicating that the flag is probably hidden within this message : 
```
( ⚆_⚆)(♥‿‿♥)󠀁󠁨󠁴󠀸󠁻󠁦󠁬󠁡󠁧󠁟󠁩󠁮󠁟󠁡󠁟󠁶󠁥󠁲󠁹󠁟󠁳󠁥󠁣󠁲󠁥󠁴󠁟󠁡󠁮󠁤󠁟󠁳󠁡󠁦󠁥󠁟󠁦󠁯󠁲󠁭󠁟󠁮󠁯󠁟󠁯󠁮󠁥󠁟󠁷󠁩󠁬󠁬󠁟󠁥󠁶󠁥󠁲󠁟󠁦󠁩󠁧󠁵󠁲󠁥󠁟󠁴󠁨󠁩󠁳󠁟󠁯󠁵󠁴󠁽󠁿(☉_☉ )
```
We can copy and paste the message into a text editor so it displays the unicode characters. We can them analyze the hexadecimal representation of the characters to find the hidden flag.

### Reflections
It was quite original to see a challenge hiding within invisible unicode characters in a discord message. It took a while for me to figure out where the flag was hidden, but it was a nice surprise when I finally found it. It was a good reminder to always look closely at the details, as sometimes the flag can be hidden in unexpected places.
  
---
[Back to home](<../README.md>)