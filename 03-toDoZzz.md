Avery wrote down things she has to do in her to-do list. But she is too tired, so instead of doing things listed on her to do list, she falls asleep. 

![](http://u.cubeupload.com/hepta/gtodo.png)

Given an array `todo`, remove all consonants for each item in the list, and replace every vowel (`a`, `i`, `u`, `e`, `o`, and `y`) with `z`. Make sure the first `z`  is capitalized. Combine all those Z's, and return it as a string. 

__Example:__
For :
```
todo = ["take a walk", 
        "make the bed", 
        "take a shower"]
```
the output should be: 
```
"ZzzzZzzzZzzzz"
```

__Explanation:__
- `"take a walk" ` contains 4 vowels, `aeaa`. Replace those 4 vowels with Z's, you'll get `"Zzzz"`.
- `"make the bed"` contains 4 vowels, `aeee`. Replace those 4 vowels with Z's, you'll get `"Zzzz"`.
- `"take a shower"` contains 5 vowels, `aeaoe`. Replace those 5 vowels with Z's, you'll get `"Zzzzz"`.

Combine them all, you'll get: `"Zzzz"` + `"Zzzz"` + `"Zzzzz"` = `"ZzzzZzzzZzzzz"`
