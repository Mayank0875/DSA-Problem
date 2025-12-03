## Title
Merchant Guilds

## Slug
merchant-guilds

## Difficulty
Medium

## Description
Cities have trade routes. A Guild is a set of cities where trade can flow cyclically.

Two cities a and b belong to the same Guild if and only if: It is possible to move from a to b, and it is also possible to move from b to a using the network of routes.
In other words, two cities are in the same Guild if they are mutually reachable.

Your task is to: Determine how many Guilds exist in total.

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
The cities form two distinct groups where round-trip traversal is possible within each group.
Cities {1, 2, 3} form one Guild.
Path: 1 -> 2 -> 3 -> 1.
Cities {4, 5} form another Guild.
Path: 4 -> 5 -> 4.
Total Guilds: 2.

### 2

#### Input
2 1
1 2

#### Output
2

#### Explanation
There are 2 cities and 1 one-way route.
Route: 1 -> 2.
One can go from 1 to 2, but not back. They form separate Guilds.

## Input Format
- The first line contains two integers n and m: the number of cities and routes.
- The following m lines describe the connections. Each line has two integers a and b, indicating a one-way route from city a to city b.

## Output Format
- Return one integer: the total number of Guilds.

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
