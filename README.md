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
