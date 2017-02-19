# Artificial Intelligence Nanodegree
## Introductory Project: Diagonal Sudoku Solver

# Question 1 (Naked Twins)
Q: How do we use constraint propagation to solve the naked twins problem?  
A: We can use constraint propagation to solve the naked twins problem by extending our reduce_puzzle function. The reduce_puzzle function applies the Eliminate Strategy and Only Choice Strategy which attempt to reduce the number of choices down to just one. The addition of Naked Twins reduces the number of possibilities that need to be searched, increases the speed of finding our final solution. Naked twins are twin digits that appear in a row or column such as '23' and '23'. Those boxes must take either the 2 or 3 so other peers in that row or column cannot take on the naked twins values ('2' or '3') eliminating a number of possibilities and consequently constraining the problem further. 

# Question 2 (Diagonal Sudoku)
Q: How do we use constraint propagation to solve the diagonal sudoku problem?  
A: We can use constraint propagation to solve the diagonal Sudoku problem through the addition of the diagonal rules. The diagonal constraint requires the solution to contain the digits 1-9 along the main diagonals of the Sudoku puzzle. The addition of this rule adds constraints to the number of possible solutions in the search.

### Install

This project requires **Python 3**.

We recommend students install [Anaconda](https://www.continuum.io/downloads), a pre-packaged Python distribution that contains all of the necessary libraries and software for this project. 
Please try using the environment we provided in the Anaconda lesson of the Nanodegree.

##### Optional: Pygame

Optionally, you can also install pygame if you want to see your visualization. If you've followed our instructions for setting up our conda environment, you should be all set.

If not, please see how to download pygame [here](http://www.pygame.org/download.shtml).

### Code

* `solutions.py` - You'll fill this in as part of your solution.
* `solution_test.py` - Do not modify this. You can test your solution by running `python solution_test.py`.
* `PySudoku.py` - Do not modify this. This is code for visualizing your solution.
* `visualize.py` - Do not modify this. This is code for visualizing your solution.

### Visualizing

To visualize your solution, please only assign values to the values_dict using the ```assign_values``` function provided in solution.py

### Data

The data consists of a text file of diagonal sudokus for you to solve.