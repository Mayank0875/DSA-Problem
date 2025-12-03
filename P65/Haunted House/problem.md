## Title
Haunted House

## Slug
haunted-house

## Difficulty
Medium

## Description
Rooms are connected by one-way secret passages. A Haunt Cycle is a group of rooms ghosts can circulate in.

Two rooms a and b belong to the same Haunt Cycle if and only if: It is possible to move from a to b, and it is also possible to move from b to a using the network of passages.
In other words, two rooms are in the same Haunt Cycle if they are mutually reachable.

Your task is to: Determine how many Haunt Cycles exist in total.

## Examples

### 1

#### Input
5 6
1 2
2 3
3 1
3 4
4 5
5 4

#### Output
2

#### Explanation
The rooms form two distinct groups where round-trip traversal is possible within each group.
Rooms {1, 2, 3} form one Haunt Cycle.
Path: 1 -> 2 -> 3 -> 1.
Rooms {4, 5} form another Haunt Cycle.
Path: 4 -> 5 -> 4.
Total Haunt Cycles: 2.

### 2

#### Input
2 1
1 2

#### Output
2

#### Explanation
There are 2 rooms and 1 one-way passage.
Passage: 1 -> 2.
One can go from 1 to 2, but not back. They form separate Haunt Cycles.

## Input Format
- The first line contains two integers n and m: the number of rooms and passages.
- The following m lines describe the connections. Each line has two integers a and b, indicating a one-way passage from room a to room b.

## Output Format
- Return one integer: the total number of Haunt Cycles.

## Constraints
- 1 ≤ n ≤ 1e5
- 1 ≤ m ≤ 2e5
- 1 ≤ a, b ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph, depth-first-search, strongly-connected-components
