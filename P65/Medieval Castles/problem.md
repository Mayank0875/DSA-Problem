## Title
Medieval Castles

## Slug
medieval-castles

## Difficulty
Medium

## Description
Castles are connected by one-way messenger roads. A Kingdom is a set of castles that can exchange messages freely.

Two castles a and b belong to the same Kingdom if and only if: It is possible to move from a to b, and it is also possible to move from b to a using the network of roads.
In other words, two castles are in the same Kingdom if they are mutually reachable.

Your task is to: Determine how many Kingdoms exist in total.

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
The castles form two distinct groups where round-trip traversal is possible within each group.
Castles {1, 2, 3} form one Kingdom.
Path: 1 -> 2 -> 3 -> 1.
Castles {4, 5} form another Kingdom.
Path: 4 -> 5 -> 4.
Total Kingdoms: 2.

### 2

#### Input
2 1
1 2

#### Output
2

#### Explanation
There are 2 castles and 1 one-way road.
Road: 1 -> 2.
One can go from 1 to 2, but not back. They form separate Kingdoms.

## Input Format
- The first line contains two integers n and m: the number of castles and roads.
- The following m lines describe the connections. Each line has two integers a and b, indicating a one-way road from castle a to castle b.

## Output Format
- Return one integer: the total number of Kingdoms.

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
