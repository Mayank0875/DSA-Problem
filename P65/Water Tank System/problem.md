## Title
Water Tank System

## Slug
water-tank-system

## Difficulty
Medium

## Description
Tanks are connected by one-way pipes. A Pressure System is a group of tanks that can circulate water among themselves.

Two tanks a and b belong to the same Pressure System if and only if: It is possible to move from a to b, and it is also possible to move from b to a using the network of pipes.
In other words, two tanks are in the same Pressure System if they are mutually reachable.

Your task is to: Determine how many Pressure Systems exist in total.

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
The tanks form two distinct groups where round-trip traversal is possible within each group.
Tanks {1, 2, 3} form one Pressure System.
Path: 1 -> 2 -> 3 -> 1.
Tanks {4, 5} form another Pressure System.
Path: 4 -> 5 -> 4.
Total Pressure Systems: 2.

### 2

#### Input
2 1
1 2

#### Output
2

#### Explanation
There are 2 tanks and 1 one-way pipe.
Pipe: 1 -> 2.
One can go from 1 to 2, but not back. They form separate Pressure Systems.

## Input Format
- The first line contains two integers n and m: the number of tanks and pipes.
- The following m lines describe the connections. Each line has two integers a and b, indicating a one-way pipe from tank a to tank b.

## Output Format
- Return one integer: the total number of Pressure Systems.

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
