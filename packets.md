# What is this?
What different packet stuff seems to be.


## Packet sizes
- 105 - Allows owner to force start game even if not everyone is in.
- 1 - Game lobby packet handler
  - Asking the host client to start game
  - Something called ready up reject
  - Undoing a ready up
  - Allowing lobby owner to force back to ability select
  - Handling player suggesting back to ability select
- 2 - Lobby init packet
- 3 - Syncs some lobby data like...
  - Player color
  - Player team
  - Player ready
- 4 - Seems to be from when a person readies up. This also appears to sync their abilities to everyone else.
   - Nothing preventing you from changing abilities mid game it appears.
