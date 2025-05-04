# Wordle-Game
Wordle Game (C++)
Overview
This is a terminal-based implementation of the popular word puzzle game Wordle. The game offers two modes: Single Player and Multiplayer. The objective is to guess a secret word within a limited number of guesses.

In Single Player mode, the player guesses a word in a certain number of attempts. In Multiplayer mode, two players take turns guessing the secret word.

The game uses a file system to select random words of different lengths (from 5 to 8 letters) and provides feedback based on the guess:

Green: The letter is in the correct position (EXACT).

Yellow: The letter is in the word but in the wrong position (CLOSE).

Red: The letter is not in the word at all (WRONG).

Features
Choose a word size between 5 and 8 letters.

Get feedback on each guess using color codes:

Green for exact matches.

Yellow for letters that are in the word but in the wrong position.

Red for letters that are not in the word.

Both Single Player and Multiplayer modes are supported.

Track the number of attempts made.

Multiplayer mode allows two players to take turns guessing.

Prerequisites
To compile and run the game, you will need:

A C++ compiler (e.g., g++ or Clang).

Standard C++ library (no external libraries are required).

A terminal that supports ANSI escape codes for color output (Linux, macOS, or Windows with an ANSI-compatible terminal).

Files
wordle.cpp: The main C++ code for the Wordle game.

5.txt, 6.txt, 7.txt, 8.txt: Word list files containing words of corresponding lengths. These files must be in the same directory as the wordle.cpp file for the game to work.

Compilation
Open your terminal and navigate to the directory containing the wordle.cpp file.

Compile the program using the following command:

bash
g++ -o wordle wordle.cpp
Run the compiled program:

bash
./wordle
Game Instructions
When you start the game, you’ll be prompted to choose a game mode:

Single Player: One player guesses the word.

Multiplayer: Two players take turns guessing the word.

Enter a word size (between 5 and 8 characters). The game will then choose a word of that size from a predefined word list.

Each player will have a limited number of attempts to guess the secret word.

After each guess, the game will provide feedback:

Green for correct letters in the correct position.

Yellow for correct letters in the wrong position.

Red for incorrect letters.

The player who guesses the word correctly in the fewest attempts wins.

If no player guesses the word correctly, the game ends with no winner.

Example Gameplay
mathematica
This is Wordle 50
Red Color Shows That the letter is not in the word
Yellow Color Shows That the letter is in the incorrect position
Green Color Shows That the letter is in the correct position

Choose game mode (S for Singleplayer, M for Multiplayer): S
Enter your name: Alice
Let's Begin Alice
You have 6 guesses
Enter a 5 letter word: table
table
[Feedback]
Correct Word for Alice: GLOSS
Better Luck Next Time
Game Logic
The game follows the basic Wordle rules, where:

The game selects a random word of the specified length from the word list.

The player enters guesses, and after each guess, the game checks if any letter is correct (EXACT), partially correct (CLOSE), or incorrect (WRONG).

The feedback is displayed using colored text, which helps the player adjust their guesses.

Notes
The game uses text files (5.txt, 6.txt, 7.txt, 8.txt) to store the words. Ensure these files are present in the same directory as the wordle.cpp file.

The color-coding system used for feedback is based on ANSI escape codes and may not render correctly on all terminals (especially on Windows unless using compatible terminals like Windows Terminal or Git Bash).

Troubleshooting
Problem: The game doesn't display colors correctly on my terminal.

Solution: Ensure you're using a terminal that supports ANSI escape codes. For Windows, use Windows Terminal or Git Bash.

Problem: The word list files are missing.

Solution: Create text files named 5.txt, 6.txt, 7.txt, and 8.txt, each containing words of the corresponding lengths. These files should be located in the same folder as the wordle.cpp source code.

License
This game is free to use and modify. Feel free to enhance or extend it as you wish!

Author
Naveed Iqbal
CT-22051
