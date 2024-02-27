# Simulated-Annealing
Develop python codes in modular fashion to perform the following functions:
Read data from the file test_data.txt. Achieve a good floorplan using Simulated Annealing algorithm. Using matplotlib or any other suitable library plot the given objects in Jupyter IDE.

Given data:
1) Number of blocks
2) An adjacency matrix representing number of wires between block i and block j. Where block i is represented in row i and block j is represented in column j of the matrix. 
3) Data of the blocks in the format {block_ID block_width block_height} 
4) Normalized Polish Expression of the initial floor plan.

Constraints: 
Assume all blocks are hard blocks with fixed dimensions, orientation of the blocks can not be changed and only one shape is available.

Cost is defined as weighted sum of area 'A' of the layout and overall wiring length 'W'. The cost C is given by C=0.75A+0.25W.
(Area) A of this layout is the area of smallest possible rectangle covering all the blocks (Wiring length) W = Summation of (cij · dij) over all i and j where cij is equal to the number of connections between blocks i and j, provided in adjacency matrix and dij is the center-to-center distance between basic rectangles i and j.

Compute the cost of initial floor plan for the initial SCORE in simulated annealing. 
Goal is to minimize this cost by applying 3 moves iteratively. 
