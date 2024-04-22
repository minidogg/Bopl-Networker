# Replay File Structure

## Header

- The header consists of a fixed 105 bytes, or 0x69 bytes.

| Byte Positions | Description | Notes |
| -------------- | ----------- | ----- |
| 0x6            | Number of players | |
| 0x7            | Number of abilities | |
| 0x2B           | Index of Player 1's color | |
| 0x33 - 0x35    | Player 1's abilities | Refer to the mapping [here](https://github.com/minidogg/Bopl-Networker/blob/main/replay.md#abilities) |
| 0x36 - 0x38    | Player 2's abilities | Refer to the mapping [here](https://github.com/minidogg/Bopl-Networker/blob/main/replay.md#abilities) |
| 0x39 - 0x3B    | Player 3's abilities | Not yet confirmed, based on assumptions from the first two players. Refer to the mapping [here](https://github.com/minidogg/Bopl-Networker/blob/main/replay.md#abilities) |
| 0x3C - 0x3E    | Player 4's abilities | Not yet confirmed, based on assumptions from the first two players. Refer to the mapping [here](https://github.com/minidogg/Bopl-Networker/blob/main/replay.md#abilities) |

## Abilities

| Hex Value | Ability Name | Notes |
| --------- | ------------ | ----- |
| 0x00      | Null         | None of your abilities, even with valid IDs, show up |
| 0x01      | Roll         | 'roll' appears as both 0x10 and 0x01 |
| 0x02      | Dash         | |
| 0x03      | Grenade      | |
| 0x04      | Bow          | |
| 0x05      | Engine       | |
| 0x06      | Blink        | |
| 0x07      | Gust         | |
| 0x08      | Growth Ray   | |
| 0x09      | Rock         | |
| 0x0A      | Missile      | |
| 0x0B      | Sword        | |
| 0x0C      | Time Stop    | |
| 0x0D      | Smoke        | |
| 0x0E      | Platform     | |
| 0x0F      | Revive       | |
| 0x10      | Roll         | roll' appears as both 0x10 and 0x01 |
| 0x11      | Shrink Ray   | |
| 0x12      | Black Hole   | |
| 0x13      | Invisibility | |
| 0x14      | Meteor       | |
| 0x15      | Macho        | |
| 0x16      | Push         | |
| 0x17      | Tesla Coil   | |
| 0x18      | Mine         | |
| 0x19      | Teleport     | |
| 0x1A      | Drill        | |
| 0x1B      | Grapple      | |
| 0x1C - 0xFF | None       | Index out of range error in BepInEx console. |
