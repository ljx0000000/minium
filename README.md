Initialization:
-------------------------------
A dp array is created to store the minimum path sums. It has the same dimensions as the input grid.
The first cell of dp is initialized to the value of the first cell of the grid.
First Row and First Column:

The first row is filled by accumulating the values from left to right.
The first column is filled by accumulating the values from top to bottom.
Dynamic Programming Transition:

For each cell (i, j), the value dp[i][j] is calculated as the minimum of the values from the cell above (dp[i-1][j]) and the cell to the left (dp[i][j-1]), plus the value of the current cell grid[i][j].

Result:
-------------------------------------
The value at the bottom-right cell dp[m-1][n-1] contains the minimum path sum from the top-left to the bottom-right corner of the grid.
You can use this code by calling the minPathSum function with your grid as input to get the minimum path sum.






