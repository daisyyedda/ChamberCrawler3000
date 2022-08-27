# Game of ChamberCrawler3000+
<img width="560" alt="Screen Shot 2022-08-27 at 7 54 25 PM" src="https://user-images.githubusercontent.com/65566095/187051821-580fd722-b4d5-4249-a65d-3d2abeea7133.png">
<br>
# Introduction
The Game of ChamberCrawler3000+ (CC3k+) is a simplified rogue-like where the player character moves through a dungeon, slays enemies, and collects treasures until reaching the end of the dungeon (the end of the 5th floor). Each floor consists of 5 chambers connected with passages. In this simplified version of CC3K+, the display is going to be terminal-based, and the player needs to type in specific commands in which the command interpreter supplies to play the game. In addition, CC3k+ differs from other rogue-likes in a significant way: it only updates the terminal/window whenever a new command has been read in, rather than updating the display in a real-time manner. 
<br>
<br>
Only the header files along with the executable are displayed here due to regulation policies, and implementation code can be provided upon request.


# PC

• human (140 HP, 20 Atk, 20 Def)

• dwarf (100 HP, 20 Atk,30 Def, gold is doubled in value)

• elves (140 HP, 30 Atk, 10 Def, negative potions have positive effect)

• orc (180 HP, 30 Atk, 25 Def, gold is worth half value)

In our game board, the player character is always denoted by the ’@’ symbol.


# Enemies

• vampire(50 HP, 25 Atk, 25 Def)

• werewolf(120 HP, 30 Atk, 5 Def)

• troll(120 HP, 25 Atk, 15 Def)

• goblin (70 HP, 5 Atk, 10 Def)

• merchant (30 HP, 70 Atk, 5 Def)

• dragon (150 HP, 20 Atk, 20 Def, always guards a treasure horde)

• phoenix (50 HP, 35 Atk, 20 Def)

Enemies are denoted on the map as follows: V(ampire), W(erewolf), N(goblin), M(erchant), D(ragon), X(Phoenix),
T(roll), M(erchant).


# Potions

Positve Potions:

• Restore health (RH): restore up to 10 HP (cannot exceed maximum prescribed by race)

• Boost Atk (BA): increase ATK by 5

• Boost Def (BD): increase Def by 5


Negative Potions:

• Poison health (PH): lose up to 10 HP (cannot fall below 0 HP)

• Wound Atk (WA): decrease Atk by 5

• Wound Def (WD): decrease Def by 5

Regardless of the potion itself, all potions are denoted on the map with a P.


# Treasure and Major Items
• normal (value 1)

• small horde (value 2)

• merchant hoard (value 4)

• dragon hoard (value 6)

Gold, regardless of type, is denoted by ’G’ on the map.

• Compass (appears once per floor, denoted by 'C')

• Barrier Suit (appears once per game, denoted by 'B')



# Command Interpreter
Initially, the game will demand the player enter one of the specified races or quit. Play will then continue in the obvious way
until the player restarts, reaches the end of floor 5, the PC dies, or the player quits. If the player reaches the end of the game
or their character is slain, give them the option of playing again. Otherwise, do the appropriate thing (restart or quit).
<br>
<br>
The following commands can be supplied to your command interpreter:

• no,so,ea,we,ne,nw,se,sw: moves the player character one block in the appropriate cardinal direction

• u ¡direction¿: uses the potion indicated by the direction (e.g. no, so, ea)

• a ¡direction¿: attacks the enemy in the specified direction, if the monster is in the immediately specified block (e.g. must be one block north of the @) 

• h, e, d, o: specifies the race the player wishes to be when starting a game

• r: restarts the game. All stats, inventory, and gold are reset. A new race should be selected

• q: allows the player to admit defeat and exit the game
<br>
<br>
Note that the board should be redrawn as appropriate every time a command is entered.
