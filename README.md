# Implement-Lee-algorithm-using-Python-
The Lee algorithm is one possible solution for maze routing problems based on Breadth-first search. It always gives an optimal solution, if one exists, but is slow and requires considerable memory.

Algorithm
1) Initialization
 - Select start point, mark with 0
 - i := 0
2) Wave expansion
 - REPEAT
     - Mark all unlabeled neighbors of points marked with i with i+1
     - i := i+1
   UNTIL ((target reached) or (no points can be marked))

3) Backtrace
   - go to the target point
   REPEAT
     - go to next node that has a lower mark than the current node
     - add this node to path
   UNTIL (start point reached)
4) Clearance
 - Block the path for future wirings
 - Delete all marks
Of course the wave expansion marks only points in the routable area of the chip, not in the blocks or already wired parts, and to minimize segmentation you should keep in one direction as long as possible.

To run this:-






*write the Python code for Lee Algorithm in Python 3.8.0 (programlee.py)



*after that we will make our maze or board in Python (maze.py)




*now we will run our file programlee.py, we get the above output









