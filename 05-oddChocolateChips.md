Avery wants to visit her parents today - and of course, her little brother. She decided to make chocolate chip cookies for him. She wants to mess around with numbers, so she separates the chocolate chips into a bunch of small groups of chocolate chips.

![](http://u.cubeupload.com/hepta/gcookie.png)

Given an array `chips` representing the total chocolate chips in each group, find out how many ways Avery can merge those groups of chocolate chips to get an odd total of chocolate chips.

__Example:__
For 
```
chips = [1, 2, 3]
```
the output should be:
```
2 
```

__Explanation:__
There are four ways to merge those groups of chocolate chips:

No  | Merged chips | Sum
---|:---:|---
1 | `[1,2]` | `3`
2 | `[1,3]` | `4`
3 | `[2,3]` | `5`
4 | `[1,2,3]` | `6`

There are two ways to merge those chocolate chips to get an odd total of chocolate chips, the 1<sup>st</sup> way, and the 3<sup>rd</sup> way.
