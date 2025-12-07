## Title
Neural Recurrence

## Slug
neural-recurrence

## Difficulty
Medium

## Description
In an artificial neural network, recurrent loops allow memory. The signal feeds back into earlier layers.

A "feedback loop" occurs when data moves from a neuron, through a sequence of weights, and returns to the starting neuron without traversing the same weight twice in immediate succession. The "length" of such a feedback loop is the number of weights it contains.

Short loops provide short-term memory. Find the size of the smallest recurrence.

Given the layout of the ANN, determine the length of the shortest feedback loop.

## Examples

### 1

#### Input
5 6
1 2
1 3
2 4
2 5
3 4
4 5

#### Output
3

#### Explanation
There are several feedback loops in this network:
1-2-4-3-1 (length 4)
2-4-5-2 (length 3)
1-2-5-4-3-1 (length 5)
The shortest feedback loop has a length of 3.

### 2

#### Input
4 3
1 2
2 3
3 4

#### Output
-1

#### Explanation
The connections form a straight line (1-2-3-4). There are no feedback loops in this network.

## Input Format
- The first line contains two integers n and m: the number of neurons and the number of weights.
- The neurons are numbered 1, 2, ..., n.
- The next m lines describe the weights. Each line contains two integers u and v, indicating a connection between neuron u and neuron v.
- The graph is undirected. There is at most one weight between any two neurons.

## Output Format
- Return one integer: the length of the shortest feedback loop. If there are no feedback loops, print `-1`.

## Constraints
- 1 ≤ n ≤ 2500
- 1 ≤ m ≤ 5000
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph, breadth-first-search
