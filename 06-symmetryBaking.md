**WARNING: description is not clear and confusing**

After arranging her chocolate chip cookies into a baking pan, Avery decides to mess around some more. This time, she counts how many *symmetrical* arrangement of cookies there were.

![](http://u.cubeupload.com/hepta/e87gckiepan.png)

Given an array`cookies` representing Avery's baking pan with her cookies in it, find how many *symmetrical* arrangements of cookies are there. Each `cookies[i]` represents the total of chocolate chips in it.

A section of cookies is considered symmetrical if:
- The arrangement of the total chocolate chips is still the same after you flip it.
- Can't consist just one cookie.

You also only can flip through either the y-axis or the x-axis.

__Example:__
For
```
cookies = [[1,1,2],
           [3,3,0],
           [1,1,2],
           [1,1,3]]
```
the output should be:
```
2
```

__Explanation:__

![Cookies explanation](http://u.cubeupload.com/hepta/cookiespan.png)

There are two ways, A and B, to flip the cookies through either the x or y axis to get the same arrangement of the total chocolate chips. The C is incorrect because the axis is neither x nor y.
