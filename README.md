# Connect-4-With-Negamax

## Project Description:
🎮 The game is played on a vertical screen with eight rows, where players take turns dropping their pieces into one of the columns. The piece falls to the lowest available position in the column, ultimately colliding with previously placed pieces. The objective is to be the first player to connect four pieces in a row horizontally, vertically, or diagonally.

<div align="center"><img src="https://github.com/HosnawHb/Connect-4-With-Negamax/blob/main/4inline.png?raw=true"width="40%"/></div> </br >

## Negamax Algorithm:
🧠 The Minimax algorithm is commonly used to solve this game, but it presents practical implementation difficulties. Instead, the alternative algorithm called Negamax is utilized. In this algorithm, at each step, the values of all child nodes are multiplied by -1, and the maximum value is assigned as the value of the parent node. Maximizing on the negatives is equivalent to minimizing, and negating the once-negative numbers in subsequent steps maximizes them.
<div align="center"><img src="https://github.com/HosnawHb/Connect-4-With-Negamax/blob/main/Negamax.png?raw=true"width="40%"/></div> </br >

## Alpha-Beta Pruning with Negamax:
⚔️ Alpha-Beta pruning, an optimization technique, can also be applied in the Negamax algorithm using the following method:
a) Consider a smaller value B as compared to A. Whenever the values of a particular node (A, B) are evaluated, if a value greater than A (the maximum value encountered so far) is found, all subsequent sibling nodes are pruned, and their calculation is skipped. The resulting interval is then multiplied by -1 and set as the value of the parent node.
b) For the root node, the initial values are set as (∞+, ∞-).
c) If a parent node has boundaries (A, B), its first child will have boundaries (B, -A). In essence, the allowed interval is multiplied by -1.
d) For each child node, except the first child, the value of the left sibling is evaluated first. If this value is D, the boundaries of this child node will be (B, D).

## Gameplay:
🔴 Upon launching the program, the game screen is displayed, and players take turns playing against each other or against the program. The current player's turn is clearly indicated on the screen. The user can select a column to place their piece in. If a player wins, the result is displayed, and the game can be restarted.

## Team Members
[Hosna Habibi](https://github.com/HosnawHb) </br>
[Pooya Kavosh](https://github.com/Jarvis017) </br>

Please refer to the code in the repository for a step-by-step guide on implementing the neural network, training the model, and evaluating its performance.
