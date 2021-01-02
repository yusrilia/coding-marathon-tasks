It's time to pack Avery's suitcase! 

![](http://u.cubeupload.com/hepta/gsuitc.png)

Given a matrix representing Avery's suitcase, determine if she can put her remaining clothes `clothes` inside her suitcase `suitcase`.
You can rotate the clothes by a multiple of 90 degrees and/or *mirror* it.

__Example:__

For
```
thing = [[0,0,1,0],
         [0,1,1,1]]

place = [[1,0,1],
         [0,0,1],
         [0,0,1]]
```

the output should be:

```
true
```

__Explanation:__

See this visualization below:

![](http://u.cubeupload.com/hepta/suit1.png)

If we rotate the `clothing` 90 degrees counter-clockwise we'll get this:

![](http://u.cubeupload.com/hepta/suit2.png)

it will fits:

![](http://u.cubeupload.com/hepta/suit3.png)
