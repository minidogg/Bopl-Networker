# information about replay files

## Header

* The header is a fixed 105, or 0x69, bytes long.

* Abilities stored for player one take up 0x33-0x35
* The first ability value is the leftmost in game, the second ability value is rightmost in game, and the third ability value is in the middle in game

quick ability table
```
00 = none of your abilities, even with valid id's, show up
01 = roll - slight anomaly, roll is in value 10 and 01
02 = dash
03 = grenade
04 = bow
05 = engine
06 = blink
07 = gust
08 = growth
09 = rock
0A = missile
0B = sword
0C = time stop
0D = smoke
0E = platform
0F =  revive
10 = roll - slight anomaly, roll is in value 10 and 01
11 = shrink
12 = black hole
13 = invisibility
14 = meteor
```
