# Scotland Yard Game

## Login

- Allow players to log in using a unique username.
- Prevent access to game features unless logged in.

---

## Main Page (Lobby)

- If the player is **not logged in**, prompt them to log in.
- If the player is **logged in**, allow them to:
  - Host a game
  - Join a game
  - Quick match

---

## Host Game

- Allow player to create a game room.
- Share room ID with others to join.
- Optionally choose number of players and rules.

---

## Quick Match

- Automatically pair players in an available room.
- If none exists, create a new one and wait for others.

---

## Join Game

- Join a game using a valid room ID.
- Handle errors for invalid or full rooms.
- Prevent joining if the game is already in progress.

---

## Assign Roles

- Randomly assign one player as **Mr. X**.
- Assign remaining players as **Detectives**.
- Notify all players of their roles.

---

## Distribute Tickets

- Distribute appropriate ticket types and quantities based on role:
  - **Mr. X**: Taxi, Bus, Underground, Secret, Double Move.
  - **Detectives**: Taxi, Bus, Underground.

---

## Player Interaction (Game Page)

- Highlight all possible routes from current location.
- After selecting a ticket, filter and highlight only valid moves.
- Display player details (name, role, current tickets, position if visible).
- Show Mr. X’s location **only on reveal turns**.
- Optional: In-game chat between players.

---

## Mr. X's Move

- Allow Mr. X to use:
  - Standard ticket
  - Secret ticket (hide transport type)
  - Double Move (2 turns in a row)
- Reveal position on specific rounds (e.g., every 3rd or 5th turn).

---

## Detective's Move

- One move per turn using available tickets.
- Cannot move to occupied spaces or without valid ticket.
- Optional :- Coordinate moves to corner Mr. X.

---

## Game End Conditions

- The game ends when:
  - Mr. X is caught (detective moves to same space).
  - 24 rounds are completed (Mr. X wins).
  - All detectives are unable to move (no valid routes or tickets).

---

## Conclude Game

- Display full travel log of Mr. X.
- Show win/loss result for all players.
- Optional:- show statistics: number of tickets used.

---

## Play Again

- Return to lobby if not continuing.
- Optional :- To play again with same group.
- Optional :- Roles can be reshuffled or kept as is.

---
