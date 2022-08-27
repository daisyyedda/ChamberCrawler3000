# Game of ChamberCrawler3000+
# Introduction
The Game of ChamberCrawler3000+ (CC3k+) is a simplified rogue-like where the player character moves through a dungeon, slays enemies, and collects treasures until reaching the end of the dungeon (the end of the 5th floor). Each floor consists of 5 chambers connected with passages. In this simplified version of CC3K+, the display is going to be terminal-based, and the player needs to type in specific commands in which the command interpreter supplies to play the game. In addition, CC3k+ differs from other rogue-likes in a significant way: it only updates the terminal/window whenever a new command has been read in, rather than updating the display in a real-time manner. 

# Command Interpreter
Initially, the game will demand the player enter one of the specified races or quit. Play will then continue in the obvious way
until the player restarts, reaches the end of floor 5, the PC dies, or the player quits. If the player reaches the end of the game
or their character is slain, give them the option of playing again. Otherwise, do the appropriate thing (restart or quit).
The following commands can be supplied to your command interpreter:
• no,so,ea,we,ne,nw,se,sw: moves the player character one block in the appropriate cardinal direction
• u ¡direction¿: uses the potion indicated by the direction (e.g. no, so, ea)
• a ¡direction¿: attacks the enemy in the specified direction, if the monster is in the immediately specified block (e.g.
must be one block north of the @)
• h, e, d, o: specifies the race the player wishes to be when starting a game
• r: restarts the game. All stats, inventory, and gold are reset. A new race should be selected.
• q: allows the player to admit defeat and exit the game.
Note that the board should be redrawn as appropriate every time a command is entered.
