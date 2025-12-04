## Title
Video Game Levels

## Slug
video-game-levels

## Difficulty
Medium

## Description
A game has N levels connected by one-way portals. A World is a set of levels that allow back-and-forth travel among them.

Two levels a and b belong to the same World if and only if: It is possible to move from a to b, and it is also possible to move from b to a using the network of portals.
In other words, two levels are in the same World if they are mutually reachable.

Your task is to: Determine how many Worlds exist in total.

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
The levels form two distinct groups where round-trip traversal is possible within each group.
Levels {1, 2, 3} form one World.
Path: 1 -> 2 -> 3 -> 1.
Levels {4, 5} form another World.
Path: 4 -> 5 -> 4.
Total Worlds: 2.

### 2

#### Input
2 1
1 2

#### Output
2

#### Explanation
There are 2 levels and 1 one-way portal.
Portal: 1 -> 2.
One can go from 1 to 2, but not back. They form separate Worlds.

## Input Format
- The first line contains two integers n and m: the number of levels and portals.
- The following m lines describe the connections. Each line has two integers a and b, indicating a one-way portal from level a to level b.

## Output Format
- Return one integer: the total number of Worlds.

## Constraints
- 1 ≤ n ≤ 1e5
- 1 ≤ m ≤ 2e5
- 1 ≤ a, b ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph, depth-first-search
