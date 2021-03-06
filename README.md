# voidgame

Void is my name for a board game I designed in college. This project is an interface for the rules of Void.

- voidgame.State holds the data. 

- voidgame.process() does the work.

```
pip install voidgame
```

## Rules of Void
Void is an abstract strategy board game for two players.

### Components and Terminology
Void is played on a circular board. The central area of the board (the void) is encircled by five concentric rings (orbits). The innermost (first) orbit is the "lowest" while the outermost (fifth) orbit is the "highest". So, in Void, "above" means "further out" and "below" means "further in". Each orbit is divided into eighteen segments (sectors). These sectors are aligned so as to form eighteen "vertical" columns of five sectors. "Orbital" means either clockwise or counter clockwise within a single orbit. "Diagonal" means equal and simultaneous change in vertical and orbital directions (ie. through the corners).

Void requires two sets (black and white) of eight pieces: one flagship, two bombers, two sweepers, and three fighters. 

_initial setup_

![Void Board Initial Setup](/pngs/void-board-initial-setup.png)

### Play
Players take turns (black first) moving one piece per turn. 

The game ends when...

- one player wins (by sending their opponent's flagship into the void)

- there is a draw (because only the two flagships remain in play)

- one player concedes

### Movement

#### The Flagship 
<img src="/pngs/void-flag-black.png" alt="Void Flagship Piece (Black)" width="100" height="100">

The flagship may move orbitally to a neighboring unoccupied sector. The flagship may not move to a new orbit. It may not move further than one sector. It may not move into an occupied sector.

After moving, the flagship may attack the first piece within three sectors along any orbital, vertical, or diagonal trajectory that belongs to the opposite color. The flagship may not attack until after it moves. It may not attack "through" an occupied sector. It may not attack further than three sectors away. It may not attack more than one piece.

When the flagship attacks, its target must fall three sectors toward the void. (ie. From the fifth orbit to the second, from the forth to the first or into the void.)

#### The Bomber 
<img src="/pngs/void-bomber-black.png" alt="Void Bomber Piece (Black)" width="100" height="100">

The bomber may move to any neighboring unoccupied sector. The bomber may not move further than one sector and it may not move into an occupied sector.

After moving, the bomber may attack all pieces directly below it. (ie. Below it in the same vertical column.) It must either attack all pieces directly below it (including pieces of the same color) or none of them.

When the bomber attacks, its target(s) must fall entirely into the void.

#### The Sweeper 
<img src="/pngs/void-sweeper-black.png" alt="Void Sweeper Piece (Black)" width="100" height="100">

The sweeper may move one sector vertically or up to seventeen sectors orbitally. The sweeper may not move diagonally. It may not move further than one sector vertically. It may not move further than seventeen sectors orbitally. It may not move to or through any occupied sector.

After moving orbitally, the sweeper may attack pieces immediately above the path of its move which belong to the opposite color. If the sweeper attacks one piece, it must also attack all other opposite-color pieces immediately above the rest of the path of its move, from the sector containing the first target piece to the sector above the sweeper.

When the sweeper attacks, its target(s) must fall two sectors toward the void.

#### The Fighter 
<img src="/pngs/void-fighter-black.png" alt="Void Fighter Piece (Black)" width="100" height="100">

The fighter may move along any single diagonal trajectory. It may not move to or through any occupied sector.

After moving along a clockwise diagonal trajectory (ie. up and clockwise or down and clockwise), the fighter may attack the first piece within two sectors clockwise if it belongs to the opposite color. After moving along a counter-clockwise diagonal trajectory (ie. up and counter-clockwise or down and counter-clockwise), the fighter may attack the first piece within two sectors counter-clockwise if it belongs to the opposite color.

When the fighter attacks, its target must fall one sector toward the void.

#### Falling
If a piece must fall through an occupied sector, the piece occupying that sector is not affected. If a piece must fall into an occupied sector, the piece occupying that sector must first fall one sector toward the void to make room. (There may be chain reactions.)

