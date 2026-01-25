## Title

The Shortest Feedback Loop

## Slug

the-shortest-feedback-loop

## Difficulty

Medium

## Description

In the high-tech world of audio engineering, feedback loops can be disastrous. You are analyzing a complex circuit board represented as a network of components and wires. Each component is a node, and each wire is a connection between two components.

A "feedback loop" occurs when a signal travels from a component, through a sequence of wires, and returns to the starting component without traversing the same wire twice in immediate succession. The "length" of such a loop is the number of wires it contains.

Long feedback loops are usually manageable, but short ones cause immediate, ear-piercing screeching. Your task is to identify the girth of the network, which is defined as the length of the shortest cycle in the graph. If the network contains no cycles, you can rest easy knowing there will be no feedback.

Given the layout of the circuit board, determine the length of the shortest cycle.

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

There are several cycles in this network:
1-2-4-3-1 (length 4)
2-4-5-2 (length 3)
1-2-5-4-3-1 (length 5)
The shortest cycle has a length of 3.
    
### 2

#### Input

4 3
1 2
2 3
3 4

#### Output

-1

#### Explanation

The connections form a straight line (1-2-3-4). There are no cycles in this network.
  

## Input Format  

- The first line contains two integers n and m: the number of components and the number of wires.
- The components are numbered 1, 2, ..., n.
- The next m lines describe the wires. Each line contains two integers u and v, indicating a connection between component u and component v.
- The graph is undirected. There is at most one wire between any two components.

## Output Format  

- Return one integer: the length of the shortest cycle (girth). If there are no cycles, print `-1`.
  

## Constraints  

- 1 ≤ n ≤ 2500
- 1 ≤ m ≤ 5000
- 1 ≤ u, v ≤ n

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

graph, hackwithinfy

## Companies
infosys