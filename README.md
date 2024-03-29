# LLM-TicTacToe
This project is a sophisticated Python-based implementation of the classic game, Tic Tac Toe. The unique aspect of this project is the utilization of two Language Learning Models (LLMs), specifically Gemini Pro and Claude 3 Opus, as the players. The entire project is encapsulated in a Jupyter Notebook, a widely used tool for executing Python code in an interactive environment.

## Code Structure

The core game logic is encapsulated within a class named `tic_tac_toe`. This class is responsible for maintaining the current state of the game and includes methods to display the game board, verify the winner or a draw, and determine the appropriate position for a player's move.

The players in this game are represented as instances of the `agent` class. The `agent` class is designed to generate a move for a player, given the current state of the game.

The primary method of the `tic_tac_toe` class is the `play()` method. This method initiates the game and manages the game loop, where the LLMs alternate turns making moves until a winner is declared or the game is determined to be a draw.

Additionally, the project includes a comprehensive data analysis of the game results using the pandas library, and visualizations using matplotlib and seaborn libraries. These analyses and visualizations provide valuable insights into the performance of the LLMs in the game.

## Execution

The line of code `tic_tac_toe().play()` serves as the entry point of the game. It creates an instance of the `tic_tac_toe` class and initiates the game by calling the `play()` method.

Upon execution of this line, the game commences, and the LLMs alternate turns to make their moves. The game continues until a winner is declared or a draw is reached. The final state of the game board is displayed at the conclusion of the game.

## Conclusion

This project provides a unique perspective on the decision-making capabilities of the LLMs in a game scenario. The included data analysis and visualizations of the game results offer valuable insights into the performance of the LLMs.

# The Battle Between LLMs ⚔️
![](https://www.googleapis.com/download/storage/v1/b/kaggle-forum-message-attachments/o/inbox%2F13602048%2F63975c34b63c3d82cc5a727f69dd669c%2FUntitled.jpg?generation=1711566697704716&alt=media)

I did a small experiment using Gemini API and Claude 3 Opus API. I made them both play Tic-Tac-Toe with each other. To my surprise Gemini API beat Claude 3 in 39 games out of 59 games !!

![](https://www.googleapis.com/download/storage/v1/b/kaggle-forum-message-attachments/o/inbox%2F13602048%2Fc7422634c7b9a4ad9d30801a140a29ba%2Foutput.png?generation=1711566879319965&alt=media) 

But there was a twist . Some time model choose the positions which was not available ,so I implemented a code that will ask the model to regenerate if such thing happens. I tracked how much time is done. Again to my surprise Gemini had to generate more than  41.5times while Claude 3 Opus had to do it 3.5 times on average.

![](https://www.googleapis.com/download/storage/v1/b/kaggle-forum-message-attachments/o/inbox%2F13602048%2Fa5474c9a90f8de1d9ef93178526b5b69%2Foutput.png?generation=1711567358460633&alt=media)

Even though I agree that the sample is very small but that was all I could do with free credits provided by Anthropic . I hope in future I may be able to expand the work to get more sample size and evaluate more models. **But still it was interesting which model understood the instruction better.**

Data For 59 Games between Claude and Gemini : https://www.kaggle.com/datasets/newtonbaba12345/the-battle-between-llms-dataset
