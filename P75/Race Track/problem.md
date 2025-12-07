## Title
Race Track

## Slug
race-track

## Difficulty
Medium

## Description
A track designer connects road segments. A race track must be a closed loop.

A "lap" occurs when a racer moves from a checkpoint, through a sequence of straightaways, and returns to the starting checkpoint without traversing the same straightaway twice in immediate succession. The "length" of such a lap is the number of straightaways it contains.

Short tracks are good for spectator visibility. Find the length of the shortest possible track layout.

Given the layout of the circuit, determine the length of the shortest lap.

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
There are several laps in this network:
1-2-4-3-1 (length 4)
2-4-5-2 (length 3)
1-2-5-4-3-1 (length 5)
The shortest lap has a length of 3.

### 2

#### Input
4 3
1 2
2 3
3 4

#### Output
-1

#### Explanation
The connections form a straight line (1-2-3-4). There are no laps in this network.

## Input Format
- The first line contains two integers n and m: the number of checkpoints and the number of straightaways.
- The checkpoints are numbered 1, 2, ..., n.
- The next m lines describe the straightaways. Each line contains two integers u and v, indicating a connection between checkpoint u and checkpoint v.
- The graph is undirected. There is at most one straightaway between any two checkpoints.

## Output Format
- Return one integer: the length of the shortest lap. If there are no laps, print `-1`.

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
