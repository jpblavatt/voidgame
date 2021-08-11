# voidgame

Void is my name for a board game I designed in college. This project is an interface for the rules of Void.

### Usage

In order to use voidgame you need to understand voidgame.State and voidgame.process().

##### State

##### process()

### Rules of Void
Void is an abstract strategy board game for two players.

##### Components and Terminology
Void is played on a circular board. The central area of the board (the void) is encircled by five concentric rings (orbits) each divided into eighteen segments (sectors). It requires two sets (black and white) of eight pieces: one flagship, two bombers, two sweepers, and three fighters. The innermost (first) orbit is the "lowest" while the outermost (fifth) orbit is the "highest". So, in Void, "above" means "further out" and "below" means "further in".

_initial setup_

![Void Board Initial Setup](/pngs/void-board-initial-setup.png)

##### Play
Players take turns (black first) moving one piece per turn. 

The game ends when...

- one player wins (by sending their oponent's flagship into the void)

- there is a draw (because only the two flagships remain in play)

- one player concedes

##### Movement

###### The Flagship 
Some rules about the flagship's movement and attack...
<img src="/pngs/void-flag-black.png" alt="Void Flagship Piece (Black)" width="200" height="200">
