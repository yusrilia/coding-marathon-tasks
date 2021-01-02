Before leaving, Avery turns off all the lamps in her apartment. The lamp switches are next to each other, and some of them were already switched off. However, they're ridiculously small. When Avery push a switch, the other two switches next to the one she pushed, will also be pushed. 

![](http://u.cubeupload.com/hepta/switch.png)

Given an array `switch` representing the lamp switches, determine if Avery could turn off all the lamps. `0` means that the lamp is off, and `1` means that the lamp is on. Note that Avery couldn't push the rightmost and the leftmost switch.

__Example:__

For

```
switch = [1, 1, 1, 0, 1, 0, 0, 1]
```

the output should be:
```
true
```

__Explanation:__

This is how Avery turn off all the switches: 
`[1, 1, 1, 0, 1, 0, 0, 1]` --> `[0, 0, 0, 0, 1, 0, 0, 1]` --> `[0, 0, 0, 0, 0, 1, 1, 1]` --> `[0, 0, 0, 0, 0, 0, 0, 0]`

