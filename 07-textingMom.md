Avery remembers that she hadn't texted his mom for a while, so she decided to do so. However, she couldn't see the letters clearly because she forgot where her glasses were, so she made typos.

![](http://u.cubeupload.com/hepta/text.png)

Given the message she sent to her mom, `message`, return the original message without typos. Avery made typos by accidentally typing the letter which is either above, below, previous to, or next to the letter she meant to type.

Assume that the keyboard looks like this:

![](http://u.cubeupload.com/hepta/kybrd.png)

And these are the rules:
- There are 4 different possible typo *directions* 
- Avery only made typos with letters.
- If a letter is lowercase, her typo stayed lowercase, if a letter is uppercase, her typo stayed uppercase.

__Example:__

For:
```
message = "Jeloo, mom."
typo    = [0, 3, 5]
dir     = "RUD"
```
the output should be:
```
"Hello, mom."
```

__Explanation:__
The first typo is at the index `typo[0]` = `0`. The 0<sup>th</sup> item (0 indexed based) of her message is `"J"`. The direction is `dir[0]` = `R`. She accidentally typed the letter at the right of the letter she meant to type. The letter she meant to type was `"h"`, so replace `"J"` with `"H"`. *(Keep the capitalization!)*

The second typo is at the index `typo[1]` = `3`. The 3<sup>rd</sup> item of her message is `"o"`. The direction is `dir[0]` = `U`. She accidentally typed the letter above the letter she meant to type. The letter she meant to type was `"l"`, so replace `"o"` with `"l"`.

The third typo is at the index `typo[2]` = `5`. The 5<sup>th</sup> item of her message is `"."`. Since `"."` is not a letter, you don't have to change anything.

__Tests:__

Input:
```
message: "Yow aee ylu?"
typo: [0, 3, 5, 9]
d: "URLD"
```

Expected Output:
```
"How are you?"
```


Input:
```
message: "I qm goid. I mkss yoy!"
typo: [1, 2, 4, 7, 10, 14, 20]
d: "UURLDDL"
```

Expected Output:
```
"I am good. I miss you!"
```

Input:
```
message: "I obly habd one unfinizhed aswigjmdng, and it's almodt cinushes."
typo: [3, 6, 9, 10, 15, 22, 29, 32, 34, 36, 38, 47, 52, 55, 58, 62, 63]
d: "LURDDDUUDDDLRDLLU"
```

Expected Output:
```
"I only have one unfinished assignment, and it's almost finished."
```

Input:
```
message: "Thankz mom!! Oh, I moas Anfre by the wqu. I womedf bow bih jr us noe."
typo: [5, 15, 18, 20, 21, 26, 29, 32, 38, 39, 40, 46, 47, 48, 49, 50, 51, 57, 58, 59, 60, 61, 62, 64, 67]
d: "DDLRLRUUURLRUDDLDRURRLLLR"
```

Expected Output:
```
"Thanks mom!! Oh, I miss Andre by the way. I wonder how big he is now."
```

Input:
```
message: "Svruakku, mom, K'm olannkjg tl so a slreplver doe tyree eayd if it'a oiay woyh you."
typo: [0, 1, 2, 5, 6, 7, 13, 15, 19, 24, 25, 29, 31, 35, 38, 41, 45, 46, 48, 51, 55, 56, 59, 66, 67, 70, 75, 76, 78, 82]
d: "RRLLLRUDLDUDLRRDRLLUDURDLURRRU"
```

Expected Output:
```
"Actually, mom, I'm planning to do a sleepover for three days if it's okay with you."
```

Input:
```
message: "Alfughg, K'll be tyere soom! Can't wait to ade hoy, dad, ajs Andfr! Hye! love you cz"
typo: [2, 3, 6, 8, 9, 13, 18, 26, 28, 34, 43, 44, 46, 47, 49, 50, 51, 55, 56, 58, 59, 60, 64, 65, 68, 71, 77, 82, 83]
d: "DLDDDDURDRLDUDLUUULULUDRULURL"
```

Expected Output:
```
"Alright, I'll be there soon! Can't wait to see you, dad, and Andre! Bye! love you xx"
```
