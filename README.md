# Trivial Compute User Guide

## Introduction

Welcome to Trivial Compute! This guide will help you understand how the game works, including set-up, gameplay mechanics, and most importantly, winning the game!

## Table of Contents

1. [Getting Started](#getting-started)
2. [Game Setup](#game-setup)
   - [Logging In or Creating an Account](#logging-in-or-creating-an-account)
   - [Creating Categories](#creating-categories)
   - [Creating Questions](#creating-questions)
   - [Exporting Questions](#exporting-questions)
   - [Creating a Game](#creating-a-game)
3. [Gameplay](#gameplay)
   - [Rolling the Dice](#rolling-the-dice)
   - [Moving Your Game Piece](#moving-your-game-piece)
   - [Answering Questions](#answering-questions)
   - [Collecting Tokens](#collecting-tokens)
4. [Winning the Game](#winning-the-game)
5. [FAQs](#faqs)

## Getting Started

Before you begin, make sure you have access to a computer with the game installed that meets the minimum hardware requirements. The game requires a minimum of an Intel Core i5 processor and 6GB of RAM to run smoothly.

## Game Setup

### Logging In or Creating an Account

1. **Launch the Game**: Open your terminal and navigate to the directory where the game is installed. Start the game by entering the following command:
   ```bash
   python3 trivial_compute_client.py
    ```
2. **Log In or Create an Account**:
    - **Log In**: If you already have an account, enter your username and password to log in.
   - **Create an Account**: If you are a new player, choose the "Create Account" option and follow the prompts to set up your username and password. Then, log into your new account to continue.

### Creating Categories

1. **Access the Category Creation Screen**: From the main menu, select "Create," then select "Create Category".
2. **Enter Category Name**: Type in the name of the category you wish to create.
3. **Save the Category**: Click the "Save Category" button. A pop-up will confirm that the category was successfully created.

### Creating Questions

1. **Access the Question Creation Screen**: From the main menu, select "Create," then select "Create Question".
2. **Enter Question Details**:
   - **Question**: Type in the trivia question.
   - **Answer**: Enter the correct answer.
   - **Category**: Choose a category from the drop-down menu to save the question under.
4. **Adding Media (Optional)**: Click the "File Upload" button, and navigate to your supported video or image file.
3. **Save the Question**: Click the "Save Question" button to save your entry.
4. **Upload Questions via CSV**: Alternatively, you can upload a CSV file containing multiple questions by clicking the "Upload CSV" button. CSV file must begin with a header and follow the format below:
   ```
   Question,Answer,Category
   How many letters are in the English alphabet?,26,Basic English,
   What is 32 divided by 8?,4,Basic Math
    ```
5. **View and Edit Questions**: Click the "View All Questions" button at the top of the question creation screen to see a list of all questions by category. You can then choose a category select a question to edit its text content.

### Exporting Questions
1. **Access the "View All Questions" Screen**: From the "Question Creation" screen, select "View All Questions," and choose a category.
2. **Export the Questions**: Clicking the "Export Questions" button on the bottom right will export all the questions for that category to CSV.


### Creating a Game

1. **Access the Game Creation Screen**: From the creation screen, select "Create Game".
2. **Set Up Game Details**:
   - **Number of Players**: Enter the number of players for the game.
   - **Select Categories**: Highlight the four categories you wish to include in the game and transfer them to the game creation list.
3. **Generate the Game**: Click the "Generate Game" button to finalize the setup.
4. **Join Code and Lobby**:
   - After generating the game, the game creator will see a join code. Share this code with players joining from separate devices.
   - On the lobby screen, each player enters their name and chooses a board marker color.

## Gameplay

### Turn Order

- Turn order is determined randomly at the start of the game.

### Moving Your Game Piece

- Use the mouse to move your game piece freely on the board, simulating a real board game experience.
- If your path crosses an intersection, you may choose which direction to go.
- If you land on a "Roll Again" space, roll the dice again and continue moving.

### Answering Questions

- When you land on a category space, such as a regular category space or a category HQ, a question corresponding to that category will appear in a pop-up window.
- After answering the question verbally, other players will determine if your answer was correct or incorrect.
- The players will select the corresponding option (correct or incorrect) in the pop-up window.

### Collecting Tokens

- If you land on a category headquarters (HQ) space and correctly answer the question, you’ll collect a token for that category.
- You can only collect one token per category.


## Winning the Game

- To win the game, you must collect a token from each of the four categories.
- After collecting all four tokens, move your game piece to the center tile on the board.
- You must land exactly on the center tile to initiate the final question.
- Once on the center tile, you will be asked a final question corresponding to one of the categories.
- If you answer the final question correctly, you win the game.
- If you answer incorrectly, your turn ends, and the game continues with the next player.


## FAQs

### How do I start a new game?

Launch the game using the command `python3 trivial_compute_client.py` in the terminal, log in or create an account, then select "Create Game" from the main menu, choose your categories, and share the game code with other players.

### Can I play the game on multiple devices?

Yes, multiple players can join the game from different computers by entering the game code.

### What happens if I answer a question incorrectly?

If you answer a question incorrectly, your turn ends, and the next player rolls the dice.

### How do I know if I’ve won?

You’ll be declared the winner once you’ve collected all four tokens and correctly answered the final question at the center tile.

### Can I edit or view existing questions?

Yes, you can view and edit existing questions by selecting "View All Questions" on the question creation screen. This allows you to manage questions within each category.

### Can I upload questions in bulk?

Yes, you can upload a CSV file containing multiple questions by selecting the "Upload CSV" button on the question creation screen. Make sure your file is formatted correctly.
