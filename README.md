java c
159.302 ARTIFICIAL INTELLIGENCE 
EXAMINATION FOR
QUESTION 1:  STATE-SPACE SEARCH [19 marks total] A robot has just made a startling discovery, while on a mission in Mars.   It has found a cure for cancer in the form. of an alien mineral.   However, its battery is almost running out and its right wheel is damaged.  In order to recharge and get immediate repair, it has to find its way back to Napoleon’s rocket ship.
The robot has to minimise energy consumption wisely, while navigating around obstacles, towards its destination.
The following cases need to betaken into account in the path calculations:
•   Turning 90° right at a junction takes time equivalent to travelling a path of length 2 (extra mechanical parts are involved in a turning action, as compared to moving straight).•   Turning 90° left at a junction takes time equivalent to travelling a path of length 3 (unfortunately, the robot’s right wheel needs to do more work to turn the robot to the left, but the right wheel is slightly damaged; therefore, it requires more energy).
All path lengths are shown in the graph.   Obstacles  are  indicated as regions coloured grey.
Hint:  For example, from B to A, the total energy cost is equal to
=  2 length units (for making a right turn) + 2 left units (actual distance indicated in the graph)
= 4 length units.
The heuristic values, associated with each node are as follows: S = 5, A= 3, B = 2, C=4, D=1, E=2, F=3, G=0.
The objective is to calculate the path that will require the least amount of energy (not the shortest distance travelled), from position S to the rocket ship (marked as node G).
Break ties alphabetically.

1.1. Search Tree 
Draw the search tree, ordering the descendants of each node alphabetically from left to right.            [2 marks]
Simulation of Search Algorithms 
General Instructions (for Parts 1.2-1.4): In your final answer, write the sequence of states expanded and the path found to the rocket ship by the specified search methods.   Indicate the state name for each step in the sequence, including S and G.
For each search method simulation, use the following table format to show your complete solution.
Step 
Dequeued 
Enqueued 
Visited List or Expanded List 
0 

(S) 

1 



…and so on 



Sequence of State Expansion:   
Path found to the rocket ship:    
1.2.     Depth-First Search without using the Visited List.   [5 marks]
1.3.     Uniform-Cost  Search   using  the  Strict   Expanded  List.  You  should  fill-in  the Expanded List column in the table. [5 marks]
1.4.    A* using the Strict  Expanded  List.  You should fill-in the Expanded List column in the table. [5 marks]
1.5. Heuristics 
Calculate the Sum of  Manhattan distance  heuristic for the given  Start state of the 8- Puzzle problem.
8-Puzzle

QUESTION 2. CONSTRAINT SATISFACTION PROBLEM [16 marks total] 
Consider assigning colours to a checkerboard so that squares that are adjacent vertically or horizontally do not have the same colour.
1 
2 
3 
4 
5 




Construct a CSP formulation of the problem according to the following requirements:
•    Let the squares be the variables and the colours be the values.
•    Limit the possible colour values to only red (R) and black (B).
• Set the initial domains of all variables equal to {R, B}.
•    Limit the colouring problem to only five squares (i.e. labelled 1, 2, 3, 4, 5), on a 3x3 board (refer to the given figure).
2.1.     Draw a constraint graph representation of the problem described.  [2 marks]
For each of the next succeeding CSP algorithm questions (Parts 2.2 – 2.5), use the following initialisation values:
• Set the initial domain of variable 5 equal to {B}.
• Set the initial domains of all the other variables equal to {R, B}.2.2.    Apply  the  full  constraint   propagation  algorithm.     Show  your  answer   using  a constraint graph.  [2 marks]
The following instruction applies to all 3 ques代 写159.302 ARTIFICIAL INTELLIGENCE EXAMINATION FORMatlab
代做程序编程语言tions 2.3, 2.4 and 2.5 below: 
As done in lectures, draw the search tree generated by the algorithm.
Stop when you reach the first solution, or the end of search tree if no solution exists.
2.3.    Apply  the  pure  backtracking  algorithm.     Show  your  answer  using  a  constraint graph.   [3 marks]
2.4.    Apply the backtracking with forward checking algorithm.  Show your answer using a constraint graph.   [4 marks]
2.5.    Apply  the   backtracking  with  forward   checking  and  dynamic  variable  ordering algorithm.  Show your answer using a constraint graph.   [5 marks]
QUESTION 3. GAMES: Min-Max and Alpha-Beta Pruning   [8 marks total] 
3.1. Simulate the MinMax algorithm on the Game Tree provided below.  Show your complete answer by filling the interior of all the nodes with the return value and the number of static evaluations.  Copy your answer (complete game tree) on the blue answer book.. 
[2 Marks]
3.2. Simulate Alpha-Beta Pruning (from left to right) on the game tree provided below.   Show  your complete  answer by filling each of the three sections of the interior of the nodes with the required information.   Copy your answer (complete game tree) on the blue answer book.

Game Tree:

QUESTION 4:  Fuzzy Logic [7 marks total] 
Consider the following FAMM with two inputs: x and y 

Fuzzy Sets = { Negative (N), Zero (ZE), Positive (P) } 
Assume  that  the  following   Fuzzy  Sets  (implemented  using  Trapezoidal  membership functions) are applicable to inputs X and Y.

For  all  the  questions  below,  refer  to  the  given  FAMM  above  and  the  corresponding numerical equivalent of the output terms.
4.1.1. Calculate the degree of membership of an input X= -0.25 to the Fuzzy set N. [1 mark]
4.1.2. Calculate the degree of membership of an input Y= 0.25 to the Fuzzy set P. [1 mark]
4.2. Given the inputs in item 5.1, calculate the degree of firing (weight) for rule #3 (i.e. W3) using Zadeh’s fuzzy AND as a logical connective.

[2 marks]4.3. Defuzzification:  Write the complete formula for calculating the centre of mass for this particular problem in terms of the weights (e.g. W1, W2, etc.) and the given outputs in linguistic terms (e.g. NL, NS, PS, etc.).   [3 marks]
QUESTION 5.  BACKPROPAGATION LEARNING [10 marks total] 

Refer to the figure depicting a multi-layer feed-forward network.  The activation and error values of the output nodes K1  and K2  have been calculated already based on the given training pattern, and  that the weights Wj1k1, Wj1k2, Wj2k1, Wj2k2 have been updated already (the adjusted weights are    shown in the figure.  Furthermore, we have the following information about the given neural network:
Learning rate η = 2
No bias nodes are used.
activation value of k1:         Ok1 = 0.67,
target output value of k1:   tk1 = 0.91
activation value of k2:         Ok2 = 0.11
target output value of k2:   tk2 = 0.01
error signal on output node k1: δk1 = 0.05
error signal on output node k2: δk2 = 0.00
activation value of node j1:           Oj1 = 0.57
training pattern:
Input: x 
Input: y 
Target output: T K1 
Target output: T K2 
1 
1 
0.91 
0.1 
Apply the given values and refer to the figure to solve for the following:
5.1. Error signal on hidden node J1: (δj1)
Write the general formula first, and then substitute the given values to find the error value.  [4 marks]
5.2. Next weight update on Wxj1 
Write the general formula first, and then substitute the given values to find the new value for the weight.  [4 marks]
Error Calculations 
Refer to the table below.  Given a neural network with 3 output nodes and a table detailing the network’s response on 3 training patterns, calculate the following error value:
5.3.          Root Mean Squared Error                                              [2 marks]

Tk – target output for output node k
Ok – actual output of output node k





         
加QQ：99515681  WX：codinghelp  Email: 99515681@qq.com
