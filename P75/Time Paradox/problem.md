## Title
Time Paradox

## Slug
time-paradox

## Difficulty
Medium

## Description
A time traveler jumps between eras. A causal loop occurs if they influence their own past.

A "causal loop" occurs when information moves from a event, through a sequence of links, and returns to the starting event without traversing the same cause-effect link twice in immediate succession. The "length" of such a causal loop is the number of links it contains.

Tight loops are the most dangerous to the timeline. Find the size of the smallest paradox.

Given the layout of the timeline, determine the length of the shortest causal loop.

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
There are several causal loops in this network:
1-2-4-3-1 (length 4)
2-4-5-2 (length 3)
1-2-5-4-3-1 (length 5)
The shortest causal loop has a length of 3.

### 2

#### Input
4 3
1 2
2 3
3 4

#### Output
-1

#### Explanation
The connections form a straight line (1-2-3-4). There are no causal loops in this network.

## Input Format
- The first line contains two integers n and m: the number of events and the number of links.
- The events are numbered 1, 2, ..., n.
- The next m lines describe the links. Each line contains two integers u and v, indicating a connection between event u and event v.
- The graph is undirected. There is at most one cause-effect link between any two events.

## Output Format
- Return one integer: the length of the shortest causal loop. If there are no causal loops, print `-1`.

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
