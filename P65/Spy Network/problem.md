## Title
Spy Network

## Slug
spy-network

## Difficulty
Medium

## Description
Spies pass dead drops. A Cell is a group of spies who can pass information to each other.

Two spies a and b belong to the same Cell if and only if: It is possible to move from a to b, and it is also possible to move from b to a using the network of drops.
In other words, two spies are in the same Cell if they are mutually reachable.

Your task is to: Determine how many Cells exist in total.

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
The spies form two distinct groups where round-trip traversal is possible within each group.
Spies {1, 2, 3} form one Cell.
Path: 1 -> 2 -> 3 -> 1.
Spies {4, 5} form another Cell.
Path: 4 -> 5 -> 4.
Total Cells: 2.

### 2

#### Input
2 1
1 2

#### Output
2

#### Explanation
There are 2 spies and 1 one-way drop.
Drop: 1 -> 2.
One can go from 1 to 2, but not back. They form separate Cells.

## Input Format
- The first line contains two integers n and m: the number of spies and drops.
- The following m lines describe the connections. Each line has two integers a and b, indicating a one-way drop from spy a to spy b.

## Output Format
- Return one integer: the total number of Cells.

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
