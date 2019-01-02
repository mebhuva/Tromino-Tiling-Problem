# Tromino-Tiling-Problem
Tromino Tiling Problem using Divide and Conquer algorithm

Given a n by n board where n is of form 2k where k >= 1 (Basically n is a power of 2 with minimum value as 2). 
The board has one missing cell (of size 1 x 1). Fill the board using L shaped tiles.
A L shaped tile is a 2 x 2 square with one cell of size 1×1 missing.

Time Complexity:
Recurrence relation for above recursive algorithm can be written as below. C is a constant.
T(n) = 4T(n/2) + C
The above recursion can be solved using Master Method and time complexity is O(n2)

How does this work?
The working of Divide and Conquer algorithm can be proved using Mathematical Induction. 
Let the input square be of size 2k x 2k where k >=1.
Base Case: We know that the problem can be solved for k = 1. We have a 2 x 2 square with one cell missing.
Induction Hypothesis: Let the problem can be solved for k-1.
Now we need to prove to prove that the problem can be solved for k if it can be solved for k-1. 
For k, we put a L shaped tile in middle and we have four subsqures with dimension 2k-1 x 2k-1 as shown in figure 2 above. So if we can solve 4 subsquares, we can solve the complete square.
