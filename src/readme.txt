Implementation of Ford Fulkerson Algorithm

Homework 2: Computing Max Flow Min Cut in a Flow Network

Programming Language: Java

@Authors:
Yash Pradhan: ypp170130

Instructions to compile and execute code:

The folder with name: ypp170130 contains java source files "FlowEdge.java", "FlowGraph.java", "FordFulkerson.java".
The driver is under main in FordFulkerson.java

Steps for running code from cmd prompt:

NOTE: while executing from command prompt, the pwd should be the directory containing the directory ypp170130.

1. Compile
> javac ypp170130/FordFulkerson.java
This would compile all files including the dependencies FlowEdge and FlowGraph.

2. Run

    2.1. Running the embedded graph example, which is the one in assignment.
    > java ypp170130/FordFulkerson

    Expected Output:

    Current Flow: 17

    Results:

    Vertices:	6
    Edges:	11

    0:  0--->1 (4/4);  0--->2 (7/7);  0--->4 (8/10);
    1:  1--->3 (0/2);  1--->5 (6/10);
    2:  2--->1 (2/2);  2--->3 (5/10);  2--->4 (0/2);
    3:  3--->5 (7/7);
    4:  4--->3 (2/2);  4--->5 (6/6);
    5:

    Max Flow: 19

    Min Cut:
    S: 0 4
    T: 1 2 3 5

    ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

    2.2. Running using custom input.
    > java ypp170130/FordFulkerson path-to-inputfile

    > java ypp170130/FordFulkerson ypp170130/graph1

    Expected Output:

    Current Flow: 0

    Results:

    Vertices:	6
    Edges:	11

    0:  0--->1 (4/4);  0--->2 (7/7);  0--->4 (8/10);
    1:  1--->3 (0/2);  1--->5 (6/10);
    2:  2--->1 (2/2);  2--->3 (5/10);  2--->4 (0/2);
    3:  3--->5 (7/7);
    4:  4--->3 (2/2);  4--->5 (6/6);
    5:

    Max Flow: 19

    Min Cut:
    S: 0 4
    T: 1 2 3 5


References:
1. Class Notes
2. Max Flow Min Cut by Robert Sedgewick: https://www.coursera.org/learn/algorithms-part2/home/week/3
