## Title
Rumor Mill

## Slug
rumor-mill

## Difficulty
Medium

## Description
In a high school, gossip spreads fast. A rumor circle is formed when gossip returns to the original source.

A "gossip chain" occurs when a story moves from a student, through a sequence of conversations, and returns to the starting student without traversing the same conversation twice in immediate succession. The "length" of such a gossip chain is the number of conversations it contains.

The shorter the chain, the faster the drama. Find the length of the shortest gossip chain.

Given the layout of the school, determine the length of the shortest gossip chain.

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
There are several gossip chains in this network:
1-2-4-3-1 (length 4)
2-4-5-2 (length 3)
1-2-5-4-3-1 (length 5)
The shortest gossip chain has a length of 3.

### 2

#### Input
4 3
1 2
2 3
3 4

#### Output
-1

#### Explanation
The connections form a straight line (1-2-3-4). There are no gossip chains in this network.

## Input Format
- The first line contains two integers n and m: the number of students and the number of conversations.
- The students are numbered 1, 2, ..., n.
- The next m lines describe the conversations. Each line contains two integers u and v, indicating a connection between student u and student v.
- The graph is undirected. There is at most one conversation between any two students.

## Output Format
- Return one integer: the length of the shortest gossip chain. If there are no gossip chains, print `-1`.

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
