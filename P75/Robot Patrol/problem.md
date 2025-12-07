## Title
Robot Patrol

## Slug
robot-patrol

## Difficulty
Medium

## Description
A security robot needs a patrol route that loops back to the charging station.

A "patrol route" occurs when the robot moves from a checkpoint, through a sequence of walkways, and returns to the starting checkpoint without traversing the same walkway twice in immediate succession. The "length" of such a patrol route is the number of walkways it contains.

Short patrols save battery. Find the length of the shortest patrol loop available.

Given the layout of the facility, determine the length of the shortest patrol route.

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
There are several patrol routes in this network:
1-2-4-3-1 (length 4)
2-4-5-2 (length 3)
1-2-5-4-3-1 (length 5)
The shortest patrol route has a length of 3.

### 2

#### Input
4 3
1 2
2 3
3 4

#### Output
-1

#### Explanation
The connections form a straight line (1-2-3-4). There are no patrol routes in this network.

## Input Format
- The first line contains two integers n and m: the number of checkpoints and the number of walkways.
- The checkpoints are numbered 1, 2, ..., n.
- The next m lines describe the walkways. Each line contains two integers u and v, indicating a connection between checkpoint u and checkpoint v.
- The graph is undirected. There is at most one walkway between any two checkpoints.

## Output Format
- Return one integer: the length of the shortest patrol route. If there are no patrol routes, print `-1`.

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
