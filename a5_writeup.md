# Assignment 5 Write up

Assignment 5 can be broken up into the following parts:
1. Import the Necessary Modules:
- `copy`: For creating deep copies of objects
- `Stack` and `Queue`: Custom implementations for DFS and BFS operations
2. Utility Functions: 
- `remove_if_exists`: Removes a specified element from a list if it exists, which is used to remove the possibilites from a cell
3. Board Class:
- Represents the Sudoku board
- Consists of functions that will find the most constrained cell, and update the board, which eliminates possible solutions
4. DFS & BFS Functions:
- `DFS`: Uses depth-first search to solve the Sudoku puzzle. It works by trying to fill the most constrained cell with potential values until a solution is found or backtracks if a mistake is made
- `BFS`: Uses breadth-first search to solve the Sudoku puzzle in a similar fashion to DFS but explores nodes level by level
5. Main Execution:
- Defines two different sets of initial moves for Sudoku puzzles
- Uses both DFS and BFS to solve each puzzle and prints the results


After completing the assignment, answer the following reflection questions:

## Reflection Questions

1. How do the performance and efficiency of the Depth-First Search (DFS) and Breadth-First Search (BFS) algorithms compare when solving Sudoku puzzles? In what scenarios might one approach be preferable over the other?
DFS differs greatly from BFS algorithms becaues it can go all the way through a perceived solution, not checking for validity until finally a contradiction in the numbers occurs. This requires much less work for the computers and can also make it much faster at times than DFS algorithms if the correct solution is identified quickly. However, if the DFS algorithm struggles to find a solution quickly, it can take very long for it to find the correct solution, leading to inconsistency. On the other hand, BFS algorithms go through every possible solution, focusing much more on accuracy but therefore creating a much slower solution process than DFS algorithms. This leads to way more consistency and accuracy, but much slower time for the computer. Therefore, DFS algorithms would be preferable for speed and less regard for consistency, whilst a BFS algorithm would be more focused on consistent, accurate results.


2. How did the choice of data structures (like the Stack for DFS and Queue for BFS) impact the implementation and functionality of the algorithms? Are there alternative data structures or design patterns that could have been used to achieve the same objectives?
Each structure navigates through data differently, therefore creating situations where Stack is more beneficial for DFS and where other data structures can become more relevant and faster for different uses. Other data structures include hashes and heaps.


3. Considering the current implementation, how might the Sudoku solver be adapted or extended for larger puzzles or different types of grid-based logic games? How can the lessons learned from this assignment be applied to real-world problem-solving or optimization challenges?
The Sudko solver could be extended for larger puzzles or different types of grid-based logic games by simply adjusting the grid size to create a larger puzzle. If the rules are different for a logic game, then the searches could be adjusted so that it can be changed to the rules of the game, as long as it conforms to the same grid-based format that Sudoku uses. This can be applied to real-world problem-solving by using the algorithms in order to chart data onto a graph and find patterns, such as weather forecasts or statistics found across the world. 