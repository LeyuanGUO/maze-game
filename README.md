# Functions applied  
  
**Basic**  
1. Initialize ncurses. Resize the terminal to a suitable size (you can decide what is suitable). Show a title screen (ask the user to start the game).  
2. In the title screen, press Enter to start the game, and press ESC to exit the game.   
3. Restore the terminal settings after quitting the game. (ncurses changes the behaviors of the terminal, say, not printing a character when pressing a keyboard key, not showing the cursor, etc. Check the example code for your reference)   
4. Press ESC during gameplay to go back to the title screen. The game is restarted when starting the game again from the title screen.   
5. Print the maze correctly (need to print the exit and the player) after the game starts.   
6. Move the player through the corridor by WSAD keys (W = up, S = down, A = left, D = right). Do not pass through walls.   
7. The player stepping on the exit wins the game. After winning the game, print a congratulation message. The player cannot be moved by pressing WSAD. Ask the user to press ESC to go back to the title screen.**Advanced Requirement**  
  
1. (2%) Random maze generation. Ensure that there exists a path to reach the exit.   
2. (2%) When the screen cannot show the whole maze, scroll the maze. (Probably you want to set some larger values for N and M, i.e., a larger maze.)   
3. (1%) Use full-width characters (i.e., using unicode) to print the maze. (So that every character is more “square”.)   
4. (1%) Limited sight! Only print a 11x11 region of the maze, centered by the player. Modify the title screen to have 3 menu items, arranged vertically. The items are “start game”, “limited sight” and “exit”. Use W and S to navigate the menu items. Press Enter to select the item. Selecting the “limited sight” menu item will toggle this game mode (without starting the game). 5. (1%) Introduce teleportation blocks, shown as the character ‘*’, in the corridor. Stepping on such a block will move the player to another random teleportation block. (Ensure that other advanced features still work if there is any)  
8. (1%) Traps! Generate spike blocks on the corridor. For every spike block, fix a random time interval. The spike will be activated after the interval, and be deactivated after another interval, and so on and so forth. When the spike is activated, it is shown as “w”. Stepping on it loses the game (See feature 7 for the requirement after losing a game). When the spike is deactivated, it is a normal corridor. The player can pass through it safely.   
9. (1%) Grab the key before leaving! A key, shown as “k” is randomly generated in the corridor. Stepping on it takes the key (and shows that the player owns the key somewhere in the game). The player must grab the key before stepping on the exit to win the game.  
11. (1%) The exit is now moving away from the player! It will move once after the player moves twice. (Find which direction can increase the “distance” from the user. The “distance” means the number of moves for the player to reach the exit)
    
**Expected score**  
Basic :         27  
Advanced :  10  
Total  :         37  
