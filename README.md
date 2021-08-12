# voidgame

Void is my name for a board game I designed in college. This project is an interface for the rules of Void.

## Usage

In order to use voidgame you need to understand voidgame.State and voidgame.process().

### State

### process()

## Rules of Void
Void is an abstract strategy board game for two players.

### Components and Terminology
Void is played on a circular board. The central area of the board (the void) is encircled by five concentric rings (orbits). The innermost (first) orbit is the "lowest" while the outermost (fifth) orbit is the "highest". So, in Void, "above" means "further out" and "below" means "further in". Each orbit is divided into eighteen segments (sectors). These sectors are aligned so as to form eighteen "verticle" columns of five sectors. "Orbital" means either clockwise or counter clockwise within a single orbit. "Diagonal" means equal and simultaneous change in vertical and orbital directions (ie. through the corners).

Void requires two sets (black and white) of eight pieces: one flagship, two bombers, two sweepers, and three fighters. 

_initial setup_

![Void Board Initial Setup](/pngs/void-board-initial-setup.png)

### Play
Players take turns (black first) moving one piece per turn. 

The game ends when...

- one player wins (by sending their oponent's flagship into the void)

- there is a draw (because only the two flagships remain in play)

- one player concedes

### Movement

#### The Flagship 
<img src="/pngs/void-flag-black.png" alt="Void Flagship Piece (Black)" width="100" height="100">
The flagship may move orbitally (either clockwise or counter-clockwise in its current orbit) to a neighboring unoccupied sector. The flagship may not move to a new orbit. It may not move further than one sector. It may not move into an occupied sector.

After moving, the flagship may attack the first piece along any orbital, vertical, or diagonal 

#### The Bomber 
<img src="/pngs/void-bomber-black.png" alt="Void Bomber Piece (Black)" width="100" height="100">
Some rules about this piece's movement and attack...

#### The Sweeper 
<img src="/pngs/void-sweeper-black.png" alt="Void Sweeper Piece (Black)" width="100" height="100">
Some rules about this piece's movement and attack...

#### The Fighter 
<img src="/pngs/void-fighter-black.png" alt="Void Fighter Piece (Black)" width="100" height="100">
Some rules about this piece's movement and attack...