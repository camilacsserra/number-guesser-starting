# Guessing Game Challenge

This project is part of the Codecademy Front End Career Path. The goal is to implement some functions in a simple guessing game using JavaScript.

## Project Overview

The project consists of writing JavaScript functions to handle the logic of a guessing game. Players (human and computer) will make guesses, and the program will determine the winner based on how close each guess is to a randomly generated target number.

## Functions Implemented

### `generateTarget`

```javascript
const generateTarget = () => Math.floor(Math.random() * 10);
```

This function generates a random target number between 0 and 9.

### `compareGuesses`

```javascript
const compareGuesses = (humanGuess, computerGuess, target) => {
    return Math.abs(humanGuess - target) <= Math.abs(computerGuess - target);
}
```

This function compares the guesses of the human player and the computer to the target number and determines the winner based on proximity. The Math.abs method returns the absolute value from the subtraction between the humanGuess or ComputerGuess and the target number.

### `updateScore`

```javascript
const updateScore = winner => {
    if (winner === 'human') {
        humanScore += 1;
    } else if (winner === 'computer') {
        computerScore += 1;
    }
}
```

This function updates the scores based on the winner of each round.

### `advanceRound`

```javascript
const advanceRound = () => {
    currentRoundNumber += 1;
}
```

This function advances the current round number.

## How to play

To play the guessing game, you can follow these steps:

1. Clone the repository.
2. Open the index.html in your preferred browser.
3. Make your guess! 