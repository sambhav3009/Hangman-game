# Hangman Game 🎉🔠

This is a command-line Hangman game written in Python. The game randomly selects a word from a word list, and the player attempts to guess the word one letter at a time. With each incorrect guess, the hangman illustration progresses until the player either guesses the word or runs out of tries.

## Table of Contents
- [Features](#features)
- [How It Works](#how-it-works)
- [Requirements](#requirements)
- [Usage](#usage)

## Features

- Randomly selects a word from a file of words.
- Uses multiple stages of Hangman illustrations to display the player's progress.
- Provides feedback after each guess and displays the current state of the word.
- Tracks the number of tries left and ends the game if the player runs out of attempts.

## How It Works

1. **Word Selection**: The game reads words from a file (`words.txt`) and randomly selects one word.
2. **Hangman Stages**: The hangman drawing progresses with each incorrect guess. Stages are read from a file (`stages.txt`), separated by `###`.
3. **Gameplay**:
   - The player guesses one letter at a time.
   - If the guess is correct, the letter appears in the word.
   - If the guess is incorrect, the number of tries decreases and the hangman drawing updates.
   - The game ends if the player guesses the entire word or runs out of tries.

## Requirements

- Python 3.x

## Usage

1. **Setup the Game Files**:
   - `words.txt`: A file containing a list of words, one per line.
   - `stages.txt`: A file containing hangman stages, separated by `###`.
2. Run the script:
   ```bash
   python hangman_game.py
