# Connect-4-With-Negamax

## Project Description:
🎮 The game is played on a vertical screen with eight rows, where players take turns dropping their pieces into one of the columns. The piece falls to the lowest available position in the column, ultimately colliding with previously placed pieces. The objective is to be the first player to connect four pieces in a row horizontally, vertically, or diagonally.

<div align="center"><img src="https://github.com/HosnawHb/Connect-4-With-Negamax/blob/main/4inline.png?raw=true"width="40%"/></div> </br >

## Negamax Algorithm:
🧠 The Minimax algorithm is commonly used to solve this game, but it presents practical implementation difficulties. Instead, the alternative algorithm called Negamax is utilized. In this algorithm, at each step, the values of all child nodes are multiplied by -1, and the maximum value is assigned as the value of the parent node. Maximizing on the negatives is equivalent to minimizing, and negating the once-negative numbers in subsequent steps maximizes them.
