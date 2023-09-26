# CLASH OF CLANS Simulation Game
Built a game simulating a basic version of Clash of Clans using OOPS concepts in python. 

## How to play: :
- To run the game : `python3 game.py`
- To view replays : `python3 replay.py`  and select the replay you want to watch according to mentioned date and time.
- For Victory : All buildings apart from walls get destroyed from the map in all three levels.
- For Defeat : If all troops and King die before destroying all buildings apart from walls.

## Controls :

### Hero :

- w : move up
- a : move left
- d : move right
- s : move down
- 1 : Special Attack
- space : Normal Attack

### Barbarian :

- z : spawn at point 1
- x : spawn at point 2
- c : spawn at point 3

### Dragon :

- v : spawn at point 1
- b : spawn at point 2
- n : spawn at point 3

### Archer :

- i : spawn at point 1
- o : spawn at point 2
- p : spawn at point 3

### Balloon :

- j : spawn at point 1
- k : spawn at point 2
- l : spawn at point 3
 
### Stealth Archers :
- t : spawn at point 1
- e : spawn at point 2
- y : spawn at point 3

#### Information / Assumptions: 

- stealth archer is a child of archer
- it contains new functions 'kill' and 'deal_damage'
- it has troop limit of 7
- it contains same attack range as archer (inheritance)

### Healers :
- u : spawn at point 1
- m : spawn at point 1
- g : spawn at point 1

#### Information / Assumptions: 

- healer is defined as a new class
- it contains functions 'move', 'find_troop', 'increase_health', 'deal_damage', 'kill', 'rage_effect', 'heal_effect'
- it has troop limit of 5
- its speed = 2, attack = 2
- healer heals everyone in its radius, and then finds next closest < max_health troop. If it cannot find a troop with health < max_health, then it does not move.

### others:
- q : Quit Game

## Bonus :

- King’s Leviathan Axe has also been implemented.
- Dragon Character has been added, it can fly over walls.
- Queen's Eagle Arrow has been added.
- Movement avoiding walls has also been implemented.
- Cannon level:
    - It gets allocated a level randomly between 1 and 5
- Wizard Tower level:
    - It gets allocated a level randomly between 1 and 5
- Wall level:
    - It also gets allocated a level randomly between 1 and 5.
    - There is commented out code for wall level = 4. This is for testing the explosion function. Uncomment this line and comment out the random allocation line.
    - Added a new function in class Wall called explosion.
    - There is a self.attack attribute which shows the damage of the explosion. It has been set to 200. 


## Assumptions :

- Rage and Heal Spell can be applied multiple times.
- The limit for troops in each level is as follows :
    - Barbarians : 10
    - Archers : 7
    - Balloon : 5
    - Dragon : 3
- You have to choose the type of troop movement at start of the game.
- You have to choose the hero after each level.