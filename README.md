         ### Battleship Project
    

    ### WOULD Framework

    ####  RequirementsAnswered
    
    
        *  Is the same console, or two different consoles working together? <div class="answers">Same console</div>
        
        *  Does the other player get one last chance after being sunk? <div class="answers">No</div>
        
        *  Do we want to capture/display stats such as hit/miss ratio etc.? <div class="answers">Just how many shots
                it took to win</div>
        
        *  Only one ship per spot. 
        *  Do we allow a player to shoot the same spot twice? <div class="answers">No</div>
        
        *  Do we show a visual of the grid? <div class="answers">Yes</div>
        
        *  Do we store game data? <div class="answers">No</div>
        
        *  Are we ever going to change number of players <div class="answers">Maybe</div>
        
        *  Will we add a computer player? <div class="answers">Maybe</div>
        
    






    #### Basic Requirements
    
        * Is the same console, or two different consoles working together? Same console
        *  Does the other player get one last chance after being sunk? No
        *  Do we want to capture/display stats such as hit/miss ratio etc.? Just how many shots it took to win
        *  Only one ship per spot. 
        *  Do we allow a player to shoot the same spot twice? No
        *  Do we show a visual of the grid? Yes
        *  Do we store game data? No
        *  Are we ever going to change number of players Maybe
        *  Will we add a computer player? Maybe
    


    #### General Flow

    
        1.  &nbsp; Two users open up the console
        1.  &nbsp; Ask user 1 where to place their ships
        1.  &nbsp; Ask user 2 where to place their ships
        1.  &nbsp; Ask user 1 for a shot
        1.  &nbsp; &nbsp; &nbsp; &nbsp;Determine hit or miss
        1.  &nbsp; &nbsp; &nbsp; &nbsp;Determine if the game is over
        1.  &nbsp; Ask user 2 for a shot
        1.  &nbsp; &nbsp; &nbsp; &nbsp;Determine hit or miss
        1.  &nbsp; &nbsp; &nbsp; &nbsp;Determine if game is over
        1.  &nbsp; Repeat until someone wins
        1.  &nbsp; Identify who the winner is
        1.  &nbsp; Exit the application
    

    #### UI Design


    
        1.  &nbsp; Welcome message
        1.  &nbsp; Add user 1 for their name
        1.  &nbsp; Add user 2 for their 5 ship placements
        1.  &nbsp; &nbsp; &nbsp; &nbsp;Ask for placement
        1.  &nbsp; &nbsp; &nbsp; &nbsp;Determine if is valid spot
        1.  &nbsp; &nbsp; &nbsp; &nbsp;Store
        1.  &nbsp; &nbsp; &nbsp; &nbsp;Clear
        1.  &nbsp; Ask user 2 for their name
        1.  &nbsp; Ask user 2 for their 5 ship placements
        1.  &nbsp; &nbsp; &nbsp; &nbsp;Ask for placement
        1.  &nbsp; &nbsp; &nbsp; &nbsp;Determine if is a valid spot
        1.  &nbsp; &nbsp; &nbsp; &nbsp;Store
        1.  &nbsp; &nbsp; &nbsp; &nbsp;Clear
        1.  &nbsp; Display grid of where user 1 is fired
        1.  &nbsp; Ask user 1: where would you like to fire on
        1.  &nbsp; &nbsp; &nbsp; &nbsp;Verify a valid spot
        1.  &nbsp; &nbsp; &nbsp; &nbsp;Check results
        1.  &nbsp; &nbsp; &nbsp; &nbsp;Store shot
        1.  &nbsp; &nbsp; &nbsp; &nbsp;Clear
        1.  &nbsp; Display the score (user 1: 2 ships left, user 2: 4 ships left)
        1.  &nbsp; Repeat with user 2
        1.  &nbsp; Loop until someone wins
        1.  &nbsp; Print out Winner's name and number of shots taken
        1.  &nbsp; Wait for the user to say they are done
        1.  &nbsp; Exit
    

    Grid Design:

    
        &nbsp; &nbsp; &nbsp; &nbsp;A1 A2 A3 O A5
        <br>
        &nbsp; &nbsp; &nbsp; &nbsp;B1 B2 B3 O B5
        <br>
        &nbsp; &nbsp; &nbsp; &nbsp;C1 C2 C3 X C5
        <br>
        &nbsp; &nbsp; &nbsp; &nbsp;D1 D2 D3 O D5
        <br>
        &nbsp; &nbsp; &nbsp; &nbsp;E1 E2 E3 O E5
    

    #### Logic Design

    
        * Clear display
        * Method: Asking for name 
        * Method: Get ship placement
        * Method: Determine if valid spot for ship
        * Storing ship information List per user?
        * Storing shot information List per user?
        * Method: create the grid for each user
        * Method: print out grid
        * Method: fire on opponent
        * Method: determine if a shot can be taken & outcome
        * Method: display score
        * Method: print winner and shots taken
    

    #### Data Design

    
        * PlayerInfo
        * User's Name
        * Users 5 ship locations: List<GridSpot>
        
        * User's shot/grid: List<GridSpot>
        
        * GridSpot
        * SpotLetter: string
        * SpotNumber: int
        * Status string (possible enum)
    
