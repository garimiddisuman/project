# Scotland Yard Game

## Login

- Allow players to log in using a unique username. [1]

```
As a player,
I want to log into the game using a unique username,
So that I can be identified and participate in the game.
```

- Allow access to game features, If logged in. [1]

```
As a returning player,
I want to be automatically logged in if my previous session is still valid,
So that I can continue playing without having to log in every time.
```

---

## Main Page (Lobby)

- If the player is **not logged in**, prompt them to log in. [1]

```
As a player,
I want pop-up window telling me to log-in,
So that I can log in to the game.
```

- If the player is **logged in**, allow them to: [1]
  - Host a game
  - Join a game
  - Quick match

```
As a player
I want match options
So that I can select the game mode that I want to play.

```

---

## Host Game

- Allow player to create a game room. [2]

```
As a player,
I want to host a game,
So that I can play with my friends.
```

- Share room ID with others to join. [2]

```
As a HOST,
I want to share the room ID,
So that other can join the game session.
```

- Optional :- choose number of players and rules.

---

## Join Game

- Join a game using a valid room ID. [1]

```
As a player,
I want to join an existing game session,
So that I can play with my friends.
```

- Handle errors for invalid or full rooms. [2]

---

## Assign Roles [1]

- Randomly assign one player as **Mr. X**.
- Assign remaining players as **Detectives**.
- Notify all players of their roles.

---

## Distribute Tickets [1]

- Distribute appropriate ticket types and quantities based on role:
  - **Mr. X**: Taxi, Bus, Underground, Secret, Double Move.
  - **Detectives**: Taxi, Bus, Underground.

---

## Player Interaction (Game Page)

- Highlight all possible routes from current location. [2]
- Highlight the currnet player pawn. [1]
- After selecting a ticket, filter and highlight only valid moves. [2]
- Display player details (name, role, current tickets, position if visible). [1]
- Show Mr. X’s location **only on reveal turns**. [1]
- Optional: In-game chat between players.

---

## Mr. X's Move

- Allow Mr. X to use:
  - Standard ticket [4]
  - Secret ticket (hide transport type) [2]
  - Double Move (2 turns in a row) [2]
- Reveal position on specific rounds (e.g., every 3rd or 5th turn).[1]

---

## Detective's Move

- One move per turn using available tickets.[4]
- Cannot move to occupied spaces or without valid ticket.[2]
- Optional :- Coordinate moves to corner Mr. X.

---

## Game End Conditions

- The game ends when:
  - Mr. X is caught (detective moves to same space). [1]
  - 24 rounds are completed (Mr. X wins).[1]
  - All detectives are unable to move (no valid routes or tickets).[4]

---

## Conclude Game

- Display full travel log of Mr. X.[2]
- Show win/loss result for all players.[2]
- Optional:- show statistics: number of tickets used.

---

## Play Again

- Return to lobby if not continuing.[1]
- Optional :- To play again with same group.
- Optional :- Roles can be reshuffled or kept as is.

---

## Quick Match [Optional]

- Automatically pair players in an available room.
- If none exists, create a new one and wait for others.

---
