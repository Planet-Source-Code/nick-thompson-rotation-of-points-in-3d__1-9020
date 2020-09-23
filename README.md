<div align="center">

## Rotation of points in 3D


</div>

### Description

This code rotates a point around another in 3D using simple fast code. It does this using x, y, z coordinates, cosine and sine. It is 100% accurate.
 
### More Info
 
oldx oldy oldz (coordinates) angle (angle of rotation in radians)

A good grasp of maths is a good idea

newx newy newz (new, rotated coordinates)

Definately no side effects


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Nick Thompson](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/nick-thompson.md)
**Level**          |Beginner
**User Rating**    |3.7 (11 globes from 3 users)
**Compatibility**  |VB 5\.0, VB 6\.0
**Category**       |[Miscellaneous](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/miscellaneous__1-1.md)
**World**          |[Visual Basic](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/visual-basic.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/nick-thompson-rotation-of-points-in-3d__1-9020/archive/master.zip)





### Source Code

```
'For best results define variables as doubles
'The angle of rotation is in Radians, view this in
'your VB help file and it will tell you how to
'convert degrees into radians
'Rotation around x-axis
 newx = oldx
 newy = (sin(angle) * oldz) + (cos(angle) * oldy)
 newz = (cos(angle) * oldz) - (sin(angle) * oldy)
'Rotation around y-axis
 newx = (cos(angle) * oldx) - (sin(angle) * oldz)
 newy = oldy
 newz = (sin(angle) * oldx) + (cos(angle) * oldz)
'Rotation around z-axis
 newx = (cos(angle) * oldx) + (sin(angle) * oldy)
 newy = (cos(angle) * oldy) - (sin(angle) * oldx)
 newz = oldz
'PS - If you have any problems with
'this please either
'e-mail me at:
'TheVBGod@Hotmail.com
'or post a comment below
' -- Thank You --
```

