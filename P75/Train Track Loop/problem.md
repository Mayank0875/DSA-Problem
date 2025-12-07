## Title
Train Track Loop

## Slug
train-track-loop

## Difficulty
Medium

## Description
A railway tycoon builds tracks. A turnaround loop allows trains to reverse direction by driving in a circle.

A "turnaround" occurs when a train moves from a station, through a sequence of tracks, and returns to the starting station without traversing the same track twice in immediate succession. The "length" of such a turnaround is the number of tracks it contains.

Tight turnarounds require less land. Find the number of track segments in the smallest loop.

Given the layout of the railway, determine the length of the shortest turnaround.

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
There are several turnarounds in this network:
1-2-4-3-1 (length 4)
2-4-5-2 (length 3)
1-2-5-4-3-1 (length 5)
The shortest turnaround has a length of 3.

### 2

#### Input
4 3
1 2
2 3
3 4

#### Output
-1

#### Explanation
The connections form a straight line (1-2-3-4). There are no turnarounds in this network.

## Input Format
- The first line contains two integers n and m: the number of stations and the number of tracks.
- The stations are numbered 1, 2, ..., n.
- The next m lines describe the tracks. Each line contains two integers u and v, indicating a connection between station u and station v.
- The graph is undirected. There is at most one track between any two stations.

## Output Format
- Return one integer: the length of the shortest turnaround. If there are no turnarounds, print `-1`.

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
