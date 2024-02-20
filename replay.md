# information about replay files

## Header

* The header is a fixed 105, or 0x69, bytes long.





| Byte positions | What they do | Notes |
| -------------- | ------------ | ----- |
| 0x6 | Controls number of players | |
| 0x7 | Number of abilities | |
| 0x2B | Index of Player 1's color | |
| 0x33 - 0x35 | Player 1's abilities | See the mapping [here](https://github.com/minidogg/Bopl-Networker/blob/main/replay.md#abilities) |
| 0x36 - 0x38 | Player 2's abilities | See the mapping [here](https://github.com/minidogg/Bopl-Networker/blob/main/replay.md#abilities) |
| 0x39 - 0x3B | Player 3's abilities | Not currently proven, just an assumtption based on the first two. See the mapping [here](https://github.com/minidogg/Bopl-Networker/blob/main/replay.md#abilities) |
| 0x3C - 0x3E | Player 4's abilities | Not currently proven, just an assumtption based on the first two. See the mapping [here](https://github.com/minidogg/Bopl-Networker/blob/main/replay.md#abilities) |

| 0x | | |









### Abilities


| Hex value | Name of ability | Notes |
| --------- | --------------- | ----- |
| 0x00 | Null | None of your abilities, even with valid id's, show up |
| 0x01 | Roll | Slight anomaly, roll is in value 10 and 01 |
| 0x02 | Dash | |
| 0x03 | Grenade | |
| 0x04 | Bow | |
| 0x05 | Engine | |
| 0x06 | Blink | |
| 0x07 | Gust | |
| 0x08 | Growth ray| |
| 0x09 | Rock | |
| 0x0A | Missile | |
| 0x0B | Sword | |
| 0x0C | Time stop | |
| 0x0D | Smoke | |
| 0x0E | Platform | |
| 0x0F | Revive | |
| 0x10 | Roll | Slight anomaly, roll is in value 10 and 01 |
| 0x11 | Shrink ray | |
| 0x12 | Black hole | |
| 0x13 | Invisibility | |
| 0x14 | Meteor | |
| 0x15 | Macho | |
| 0x16 | Push | |
| 0x17 | Tesla coil | |
| 0x18 | Mine | |
| 0x19 | Teleport | |
| 0x1A | Drill | |
| 0x1B | Grapple | |
| 0x1C - 0xFF | None | Index out of range error in BepInEx console. |


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
0F = revive
10 = roll - slight anomaly, roll is in value 10 and 01
11 = shrink
12 = black hole
13 = invisibility
14 = meteor
```
