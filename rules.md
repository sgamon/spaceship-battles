# Spaceship Battles

A game about combat between spaceships in a science fiction future.


## I. Introduction

Spaceship Battles is a set of rules for a paper wargame. There are rules for 
designing spaceships, and rules for fighting between spaceships.

Players must provide:

* one 6-sided die
* a hex grid
* ship markers, with a facing (ie, it should be clear which direction the ship
is pointing)
* paper and pencil, to design ships and record damage


## II. Sequence of Play

### A. Initiative

1. Players roll for Initiative. High roll wins.

### B. Movement

1. Players alternate moving ships. Player _without_ Initiative goes first.

### C. Combat

1. Players alternate firing volleys (see IV.A) at each other. Player _with_ 
Initiative goes first. Damage takes effect immediately.


## III. Movement

### A. Speed

1. A ship may move as many hexes as it has engines. It may move some, none, or 
all of this speed, every turn.

### B. Turning

1. A ship must always face a hexside. When moving, it must always move into the 
hex directly ahead.
2. To turn, a ship must first move forward a number of hexes equal to its turn 
mode. It may then spin and face of the the hexsides adjacent to the hexside it 
is facing.


## IV. Combat

### A. Volleys

1. A volley consists of all the weapons fired by a single ship, at another 
single ship.
2. Ships equipped with DataLink can form fire groups of up to 3 ships. Fire 
groups may fire simultaneously on a common target, with their fire considered 
a single volley.
3. Ships with Multiplex Tracking can fire on moer than 1 target ship with 
their volley. 
4. A ship may not use DataLink and Multiplex Tracking in the same volley.
5. Weapons can only volley fire at targets in their arc of fire.

### B. Hit Procedure

1. The firing player cross-indexes the range to the target with the result of 
1 die on the appropriate chart, repeating this action for each weapon fired. 
The result is the number of damage points inflicted on the target.
2. Point Defense systems will attempt to shoot down all missiles which hit. For 
each missle that hits, cross reference the result of 1 die with the total 
number of missles that hit. A hit destroys the missle before it inflicts damage.

### C. Damage

1. The owner of a target ship crosses out one system for each damage point 
received. Cross these out from left to right as they appear on the 
Ship Code.
2. Energy Beam damage skips over armor and cargo. Cross out the next system 
(that is not armor or cargo).
3. Primary Beam damage skips over shields and armor. 

### D. Tractor Beams

1. After all other volleys have been fired, Tractor Beams may fire.
2. If the throw of 1 die exceeds the maximum speed of the target ship, then a 
hit as been scored. Add the target's turn mode, and subtract the range from the 
die. Max range is 5.
3. A hit cannot be achieved on a ship with Shear Plane.
4. If a hit is scored, neither ship may move during the next turn. Instead, 
both ships will move one hex closer together.
5. The ship with the tractor beam enjoys a +1 dm on all volleys against the 
affected target.
6. Step 2 must be repeated each turn.

### E. Overload Dampers

1. Overload Dampers can absorb 1 point of damage per volley from an Energy Beam.
Alternately, it may absorb up to 4 points at the cost of burning out (cross 
out the system).

### F. Primary Beams

1. Primary Beams may only be fired ever-other-turn.
2. As noted above (see IV.C.3), Primary Beams skip over shields and armor. 
Randomly select any other system to cross out.


## V. Ship Design

#### A. Procedure

The Hull Table lists the class, space available, turn mode, cost per 
engine, and space per engine for each Hull type.

The Component Table lists the System Code (aka "SC"), cost, and space used for 
each system.

1. First, purchase a Hull. Then purchase engines. A ship may have no more than 
6 engines. Next, buy as many components as you please, so long as it all fits 
in the ship. Finally, make up a Ship Code for each ship.
2. Each weapon must be assigned to an arc of fire: front (f), right (r), 
left (l), rear (b).
3. Each Advanced Maneuvering system reduces the ship's turn mode by 1. Advanced 
Maneuvering costs 10% of the Hull cost (rounded down to a whole number). The 
turn mode may not be reduced to less than 1.

#### B. Ship Codes

A Ship Code is a terse way to describe a ship design.

The layout of a Ship Code is:

    [class]-[system codes]-[cost]-[turn mode]-[engines]
    
Example:

    E-SAI(Gf)I(Xf)IIV-84-1-4

1. Class: the Hull code.
2. System codes: List the system codes in any order. Since they are destroyed 
sequentially in combat, order is signifcant. Weapons are listed in parens, and 
include the facing code.
4. Cost: total points
5. Turn mode: Final turn mode after accounting for any Advanced Maneuvering. 
As Advanced Maneuvering systems are lost in combat, cross this out and adjust 
it.
6. Engines: number of engines, which is the starting speed of the ship. As 
engines are lost in combat, cross this out and adjust it.

#### C. Design Tables

1. Hull Table

|Class            |Code|Spaces|Turn Mode|Cost|Engine Cost|Engine Space|AM* |
|-----------------|----|------|---------|----|-----------|------------|----|
|Escort           |E   |10    |2        |33  |5          |.5          |3   |
|Corvette         |C   |13    |2        |60  |5          |.5          |6   |
|Frigate          |F   |17    |2        |72  |5          |1           |7   |
|Destroyer        |D   |25    |3        |123 |8          |1           |12  |
|Cruiser          |CR  |50    |3        |300 |8          |2           |30  |
|Battlecruiser    |BC  |70    |4        |360 |12         |2           |36  |
|Battleship       |BS  |80    |4        |486 |12         |3           |48  |
|Super Dreadnought|SD  |120   |5        |816 |7          |3           |81  |

*AM = cost per Advanced Maneuvering system

2. Component Table

|Code|System              |Cost|Space|
|----|--------------------|----|-----|
|G   |Gun                 |5   |3    |
|M   |Missile             |10  |3    |
|X   |Gun/Missile         |20  |3    |
|F   |Force Beam          |25  |4    |
|L   |Laser Beam          |30  |4    |
|E   |Energy Beam         |40  |4    |
|P   |Primary Beam        |50  |4    |
|A   |Armor               |2   |1    |
|S   |Shield              |4   |1    |
|O   |Overload Damper     |20  |1    |
|Y   |Point Defense       |25  |2    |
|C   |Cargo               |0   |5    |
|U   |Multiplex Tracking  |30  |2    |
|D   |DataLink            |40  |0    |
|R   |Tractor Beam        |9   |2    |
|H   |Shear Plane         |15  |2    |
|V   |Advanced Maneuvering|*   |0    |
|I   |Engine              |*   |*    |

*see Hull Table

## VI. Combat Tables

1. Gun

|Range/Die|1-2|3-4|5-6|7-8|9-10|
|---------|---|---|---|---|----|
|    1    | - | - | - | - | -  |
|    2    | 1 | - | - | - | -  |
|    3    | 1 | 1 | - | - | -  |
|    4    | 1 | 1 | 1 | - | -  |
|    5    | 1 | 1 | 1 | 1 | -  |
|    6    | 1 | 1 | 1 | 1 | 1  |

2. Missile

|Range/Die|1-2|3-6|7-11|12-15|16-20|
|---------|---|---|----|-----|-----|
|    1    | - | - | -  |  -  |  -  |
|    2    | - | 1 | -  |  -  |  -  |
|    3    | - | 1 | 1  |  -  |  -  |
|    4    | - | 1 | 1  |  1  |  -  |
|    5    | - | 1 | 1  |  1  |  1  |
|    6    | 1 | 1 | 1  |  1  |  1  |


3. Point Defense

|Hits/Die | 1 |2-3|4-5|6+ |
|---------|---|---|---|---|
|    1    | - | - | - | - |
|    2    | 1 | - | - | - |
|    3    | 1 | 1 | - | - |
|    4    | 1 | 1 | 1 | - |
|    5    | 1 | 1 | 1 | 1 |
|    6    | 1 | 1 | 1 | 1 |

4. Force Beam

|Range/Die|1-2|3-6|7-10|11-17|
|---------|---|---|----|-----|
|    1    | - | - | -  |  -  |
|    2    | 5 | - | -  |  -  |
|    3    | 5 | 1 | -  |  -  |
|    4    | 5 | 1 | 1  |  -  |
|    5    | 5 | 1 | 1  |  .5 |
|    6    | 5 | 1 | 1  |  .5 |

5. Laser Beam

|Range/Die|1-3|4-6|7-9|
|---------|---|---|---|
|    1    | - | - | - |
|    2    | 2 | - | - |
|    3    | 2 | 1 | - |
|    4    | 2 | 1 |.5 |
|    5    | 2 | 1 |.5 |
|    6    | 2 | 1 |.5 |

6. Energy Beam

|Range/Die|1-3|4-6|7-9|
|---------|---|---|---|
|    1    | - | - | - |
|    2    | 3 | - | - |
|    3    | 4 | 1 | - |
|    4    | 4 | 2 |.5 |
|    5    | 5 | 2 |.5 |
|    6    | 5 | 3 | 1 |


7. Primary Beam

|Range/Die|1-2|3-6|7-10|11-14|
|---------|---|---|----|-----|
|    1    | - | - | -  |  -  |
|    2    | 1 | - | -  |  -  |
|    3    | 1 | 1 | -  |  -  |
|    4    | 1 | 1 | 1  |  -  |
|    5    | 1 | 1 | 1  |  .5 |
|    6    | 1 | 1 | 1  |  .5 |
