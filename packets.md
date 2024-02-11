# What is this?
What different packet stuff seems to be.


## Packet sizes
- 105 - Allows owner to force start game even if not everyone is in.
- 1 - Game lobby packet handler
  - Asking the host client to start the game
  - Something called ready up reject
  - Undoing a ready up
  - Allowing lobby owner to force back to ability select
  - Handling player suggesting back to ability select

- 3 - Syncs some lobby data like...
  - Player color
  - Player team
  - Player ready
- 4 - Seems to be from when a person readies up. This also appears to sync their abilities to everyone else.
   - Nothing prevents you from changing abilities mid-game it appears.
- 15 - Appears to do a lot of stuff related to syncing
   - Makes sure a player's color is only used once.
   - Syncs pretty much every option in the ability select.
- 2 - Lobby init packet
   - Really short which makes it hard to understand anything else about it
- 6 - Ping/ACK
   - Seems to get ping
   - Sends an ACK
