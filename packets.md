# What is this?
What different packet stuff seems to be.


## Packet sizes
- 105 - Game start packet
  - Sent by the host to start the game.
  - Syncs all of the teams, abilities, and colors (the reason why it's so big)
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
   - The first byte is the number of abilities and the second byte is a buffer byte to distinguish it from the first packet size
- 6 - ACK
   - Sent every frame either to the clients either to ping or acknowledge a sent ping (5 for ping and 6 for a ping acknowledgement)
