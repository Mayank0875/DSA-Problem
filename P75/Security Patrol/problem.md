## Title
Security Patrol

## Slug
security-patrol

## Difficulty
Medium

## Description
Guards walk beats. A beat is a circular path covering specific stations.

A "beat" occurs when a guard moves from a station, through a sequence of paths, and returns to the starting station without traversing the same path twice in immediate succession. The "length" of such a beat is the number of paths it contains.

Short beats allow frequent checks. Find the length of the shortest patrol beat.

Given the layout of the compound, determine the length of the shortest beat.

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
There are several beats in this network:
1-2-4-3-1 (length 4)
2-4-5-2 (length 3)
1-2-5-4-3-1 (length 5)
The shortest beat has a length of 3.

### 2

#### Input
4 3
1 2
2 3
3 4

#### Output
-1

#### Explanation
The connections form a straight line (1-2-3-4). There are no beats in this network.

## Input Format
- The first line contains two integers n and m: the number of stations and the number of paths.
- The stations are numbered 1, 2, ..., n.
- The next m lines describe the paths. Each line contains two integers u and v, indicating a connection between station u and station v.
- The graph is undirected. There is at most one path between any two stations.

## Output Format
- Return one integer: the length of the shortest beat. If there are no beats, print `-1`.

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
