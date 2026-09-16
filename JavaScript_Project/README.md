# JavaScript Slot Machine Project

# Overview

This project is a command-line slot machine built with JavaScript. The game allows the player to deposit money, choose the number of lines to bet on, place a wager, spin the reels, and earn winnings based on matching symbols. The program includes input validation, balance tracking, payout calculations, and a replay loop to create a complete casino-style experience.

The project was developed in a structured, step-by-step approach, beginning with the project setup and then progressing through the core gameplay logic. It includes the necessary dependency setup, slot configuration, reel generation, win evaluation, and final game flow.

# Project Goals

The main goal of this project was to recreate the mechanics of a slot machine in a simple JavaScript application. The game follows a realistic flow:

- Deposit money into the game
- Choose how many lines to play
- Enter a bet amount per line
- Spin the slot machine
- Check for matching symbols
- Calculate winnings
- Update the player balance
- Continue playing until the balance is empty or the player exits
- Features
- Secure and simple deposit validation
- Line selection with a limited range
- Bet validation based on the current balance
- Randomized symbol generation for the reels
- Row and column-based slot layout
- Win detection for matching symbol patterns
- Balance updates after each spin
- Restart prompt after each round
- Game loop that ends when the player runs out of money
- Setup and Dependencies
- The project includes the required package configuration and dependency setup needed to run the game successfully.

- JavaScript application logic is contained in the main project file
- Package configuration was created to manage the project and dependencies
- The project uses the prompt-sync package to collect user input in the terminal
- A lock file was also generated to maintain a consistent dependency version for the project
- Slot Configuration
- The game includes the slot machine structure and payout settings:

Rows: 3
Columns: 3
Symbol set: A, B, C, D
Symbol counts and values were assigned to determine how often each symbol appears and how much it pays when matched
This configuration is essential for establishing the reel probabilities and win values used throughout the game.

Game Logic Summary
The implementation includes several core functions that work together to create the full gameplay experience:

deposit(): Prompts the player to enter a valid deposit amount and checks for invalid values
getNumberOfLines(): Allows the player to choose between 1 and 3 lines
getBet(): Validates the wager amount against the current balance and selected number of lines
spin(): Generates a random set of symbols for each reel
transpose(): Organizes the reel results into rows for display
printRows(): Displays the slot rows in the terminal
getWinnings(): Calculates payout based on matching symbols across the selected lines
game(): Runs the main application flow, updates the balance, and asks if the player wants to continue
Winning System
The winnings are calculated by checking each active row to determine whether all symbols match. If a row contains the same symbol across the selected positions, the player receives a payout based on the symbol value and the current bet amount. The balance is then updated to reflect the result of the spin.

Player Experience
The game keeps the player informed at each stage by presenting messages that show:

Current balance
Deposit amount
Number of lines selected
Bet per line
Spin results
Winnings earned
Whether the player has run out of money
Whether they want to play again
This creates an interactive and complete game loop that is easy to follow and play.

Author
Matthew D. Mayer

Conclusion
This JavaScript slot machine project demonstrates a practical use of logic, loops, conditionals, randomization, and game-state management. It combines a clean game flow with input validation and reward logic to deliver a complete, playable slot machine experience in the terminal.