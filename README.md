# Mancala AI Player Project

## Introduction

This project is part of the CSCI 3202 course, designed to showcase concepts and skills in artificial intelligence by developing an AI application for the game of Mancala. The project includes implementing different AI algorithms, such as Minimax and Alpha-Beta pruning, to compete against a random player, aiming to outperform random decisions through strategic gameplay.

## Project Objectives

The project involves multiple steps to create an AI player for Mancala, test its performance, and compare it with a random opponent. The following key objectives were set:

- **Implement Mancala Game**: Develop an interface that allows two participants to play our version of Mancala, including random opponents.
- **Random Player**: Create a player that selects moves randomly to provide a benchmark for evaluating the AI player.
- **Minimax AI Player**: Construct an AI player using the Minimax algorithm with a utility function that evaluates game outcomes.
- **Alpha-Beta AI Player**: Develop a second AI player using the Alpha-Beta pruning technique to enhance search efficiency.
- **Performance Evaluation**: Test both AI players against the random player in different scenarios, including adjusting the search depth (plies), and analyze their performance metrics.

## Mancala Rules

This project uses modified Mancala rules:

- Players take turns selecting pits on their side of the board containing stones and distribute them in a counter-clockwise direction.
- If the last stone lands in the player’s empty pit and the opponent’s pit has stones, the player collects all the stones.
- The game ends when all pits on one side are empty; the player with the most stones in their Mancala wins.

## Project Components

- **Random Player vs. Random Player**: Conducted simulations to establish a baseline for gameplay without strategic AI. Both players were expected to win roughly 50% of the time.
- **Minimax AI Player**: Implemented Minimax AI to evaluate game states and choose optimal moves based on a utility function. We used the AIMA library and customized the game tree evaluation.
- **Alpha-Beta Pruning AI Player**: Added Alpha-Beta pruning to the Minimax algorithm to enhance search speed, especially for larger tree depths.
- **Performance Analysis**: Evaluated the performance of both AI players against a random opponent, considering metrics like win rate, average number of moves, and computation time.

## Results

- The Minimax AI Player at a depth of 5 plies was consistently able to outperform the random player, achieving a win rate greater than 50%.
- The Alpha-Beta Pruning AI Player showed similar results to the Minimax AI but with improved efficiency in terms of search time.
- Increasing the number of plies improved AI performance but led to longer computation times.

## Libraries and Frameworks Used

- **Python and Jupyter Notebook**: For implementation and testing.
- **AIMA Python Library**: Used for Minimax and Alpha-Beta algorithms.

## How to Run

To run the project, clone the repository and open the notebook file `mancala_ai_project.ipynb` in Jupyter. Follow the instructions in the notebook to simulate games between the AI and random players.

### Requirements

- Python 3.x
- Jupyter Notebook
- AIMA library (`pip install aima-python`)

## Conclusion

This project demonstrates the effectiveness of AI in decision-making for traditional board games. The Minimax and Alpha-Beta AI players effectively learned to play Mancala, outperforming a random opponent in a majority of games. Further improvements could involve integrating reinforcement learning for better strategy development.

## Acknowledgements

- **University of Colorado Boulder** - For providing guidance and resources for the course project.
- **AIMA Team** - For the Python library used to implement the algorithms.
