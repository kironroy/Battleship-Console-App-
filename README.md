### Battleship Project

### WOULD Framework
#### Basic Requirements

*   Is the same console, or two different consoles working together? Same console
*   Does the other player get one last chance after being sunk? No
*   Do we want to capture/display stats such as hit/miss ratio etc.? Just how many shots it took to win
*   Only one ship per spot.
*   Do we allow a player to shoot the same spot twice? No
*   Do we show a visual of the grid? Yes
*   Do we store game data? No
*   Are we ever going to change number of players Maybe
*   Will we add a computer player? Maybe

#### Requirements Answered

*   Is the same console, or two different consoles working together?
    
    Same console
    
*   Does the other player get one last chance after being sunk?
    
    No
    
*   Do we want to capture/display stats such as hit/miss ratio etc.?
    
    Just how many shots it took to win
    
*   Only one ship per spot.
*   Do we allow a player to shoot the same spot twice?
    
    No
    
*   Do we show a visual of the grid?
    
    Yes
    
*   Do we store game data?
    
    No
    
*   Are we ever going to change number of players
    
    Maybe
    
*   Will we add a computer player?
    
    Maybe
    


#### General Flow

1.  Â  Two users open up the console
2.  Â  Ask user 1 where to place their ships
3.  Â  Ask user 2 where to place their ships
4.  Â  Ask user 1 for a shot
5.  Â  Â  Â  Â Determine hit or miss
6.  Â  Â  Â  Â Determine if the game is over
7.  Â  Ask user 2 for a shot
8.  Â  Â  Â  Â Determine hit or miss
9.  Â  Â  Â  Â Determine if game is over
10.  Â  Repeat until someone wins
11.  Â  Identify who the winner is
12.  Â  Exit the application

#### UI Design

<<<<<<< HEAD
1.    Welcome message
2.    Add user 1 for their name
3.    Add user 1 for their 5 ship placements
4.         Ask for placement
5.         Determine if is valid spot
6.         Store
7.         Clear
8.    Ask user 2 for their name
9.    Ask user 2 for their 5 ship placements
10.         Ask for placement
11.         Determine if is a valid spot
12.         Store
13.         Clear
14.    Display grid of where user 1 is fired
15.    Ask user 1: where would you like to fire on
16.         Verify a valid spot
17.         Check results
18.         Store shot
19.         Clear
20.    Display the score (user 1: 2 ships left, user 2: 4 ships left)
21.    Repeat with user 2
22.    Loop until someone wins
23.    Print out Winner's name and number of shots taken
24.    Wait for the user to say they are done
25.    Exit
=======
1.  Â  Welcome message
2.  Â  Add user 1 for their name
3.  Â  Add user 1 for their 5 ship placements
4.  Â  Â  Â  Â Ask for placement
5.  Â  Â  Â  Â Determine if is valid spot
6.  Â  Â  Â  Â Store
7.  Â  Â  Â  Â Clear
8.  Â  Ask user 2 for their name
9.  Â  Ask user 2 for their 5 ship placements
10.  Â  Â  Â  Â Ask for placement
11.  Â  Â  Â  Â Determine if is a valid spot
12.  Â  Â  Â  Â Store
13.  Â  Â  Â  Â Clear
14.  Â  Display grid of where user 1 is fired
15.  Â  Ask user 1: where would you like to fire on
16.  Â  Â  Â  Â Verify a valid spot
17.  Â  Â  Â  Â Check results
18.  Â  Â  Â  Â Store shot
19.  Â  Â  Â  Â Clear
20.  Â  Display the score (user 1: 2 ships left, user 2: 4 ships left)
21.  Â  Repeat with user 2
22.  Â  Loop until someone wins
23.  Â  Print out Winner's name and number of shots taken
24.  Â  Wait for the user to say they are done
25.  Â  Exit
>>>>>>> 4d9a70e65ae0d6574bdb1c0b04c8cfaf44c70d27

Grid Design:

Â  Â  Â  Â A1 A2 A3 O A5  
Â  Â  Â  Â B1 B2 B3 O B5  
Â  Â  Â  Â C1 C2 C3 X C5  
Â  Â  Â  Â D1 D2 D3 O D5  
Â  Â  Â  Â E1 E2 E3 O E5

#### Logic Design

*   Clear display
*   Method: Asking for name
*   Method: Get ship placement
*   Method: Determine if valid spot for ship
*   Storing ship information List per user?
*   Storing shot information List per user?
*   Method: create the grid for each user
*   Method: print out grid
*   Method: fire on opponent
*   Method: determine if a shot can be taken & outcome
*   Method: display score
*   Method: print winner and shots taken

#### Data Design

*   PlayerInfo
*   User's Name
*   Users 5 ship locations: List
*   User's shot/grid: List
*   GridSpot
*   SpotLetter: string
*   SpotNumber: int
*   Status string (possible enum)
<<<<<<< HEAD

=======
>>>>>>> 4d9a70e65ae0d6574bdb1c0b04c8cfaf44c70d27
