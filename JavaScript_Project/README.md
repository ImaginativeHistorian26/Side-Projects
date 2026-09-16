# JavaScript Slot Machine Project

## Overview

This project is a command-line slot machine game built with JavaScript. It allows the player to deposit money, choose the number of lines to bet on, place a wager, spin the reels, and earn winnings based on matching symbols. The game includes input validation, balance tracking, payout calculations, and a replay loop to create a complete slot machine experience.

The project was developed in a structured, step-by-step process, beginning with the setup and continuing through the core game logic. It includes the necessary configuration, reel generation, symbol setup, payout logic, and final gameplay flow.

## Project Purpose

The goal of this project was to recreate a slot machine in JavaScript while applying fundamental programming concepts such as variables, loops, conditionals, arrays, functions, and randomization. The result is a playable terminal-based game that simulates betting, spinning, and winning.

## Features

- Validates deposit amounts to ensure only positive numeric values are accepted
- Allows the user to select the number of lines to bet on
- Checks the bet amount against the player's available balance
- Generates random symbols for each reel
- Displays a 3x3 slot layout
- Calculates winnings based on matching symbols across selected lines
- Updates the balance after each turn
- Prompts the user to continue playing after each round
- Ends the game when the player runs out of money

## Project Setup

This project includes the necessary package configuration and dependency setup required to run the game successfully. The application uses the `prompt-sync` package to collect terminal input, and the project lock file was created to maintain consistent dependency versions.

## Slot Machine Configuration

The game is built around a standard slot machine setup:

- Rows: 3
- Columns: 3
- Symbols: A, B, C, D
- Symbol counts and values were defined to determine reel probabilities and payout amounts

## Core Game Logic

The project is organized into several key functions:

- `deposit()`: prompts the player for a valid deposit amount
- `getNumberOfLines()`: validates how many lines the player wants to bet on
- `getBet()`: checks that the wager is valid based on the current balance
- `spin()`: randomly generates symbols for the reels
- `transpose()`: rearranges reel data into rows for display
- `printRows()`: prints the slot rows to the console
- `getWinnings()`: calculates the payout for matching rows
- `game()`: manages the main game flow and replay loop

## How the Game Works

1. The player deposits money.
2. The player chooses how many lines to play.
3. The player enters a bet amount per line.
4. The slot machine spins and generates random symbols.
5. The results are displayed in rows.
6. Matching symbols determine whether the player wins.
7. Winnings are added to the balance.
8. The player is asked whether they want to continue.
9. The game ends when the balance reaches zero or the player exits.

## User Experience

The game keeps the player informed throughout each round by displaying the current balance, selected number of lines, bet amount, spin results, and winnings. It also includes validation messages for invalid input, helping create a more interactive and user-friendly experience.

## Author

Matthew D. Mayer

## Conclusion

This project demonstrates the practical application of JavaScript fundamentals in a real game environment. By combining logic, randomization, validation, and game flow, it creates a complete and playable slot machine experience in the terminal.