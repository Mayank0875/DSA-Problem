## Title
Chemical Reaction Cycles

## Slug
chemical-reaction-cycles

## Difficulty
Medium

## Description
Chemical substances can transform into others via one-way reactions. A Reaction Cycle is a group of substances that can interconvert indefinitely.

Two substances a and b belong to the same Reaction Cycle if and only if: It is possible to move from a to b, and it is also possible to move from b to a using the network of reactions.
In other words, two substances are in the same Reaction Cycle if they are mutually reachable.

Your task is to: Determine how many Reaction Cycles exist in total.

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
The substances form two distinct groups where round-trip traversal is possible within each group.
Substances {1, 2, 3} form one Reaction Cycle.
Path: 1 -> 2 -> 3 -> 1.
Substances {4, 5} form another Reaction Cycle.
Path: 4 -> 5 -> 4.
Total Reaction Cycles: 2.

### 2

#### Input
2 1
1 2

#### Output
2

#### Explanation
There are 2 substances and 1 one-way reaction.
Reaction: 1 -> 2.
One can go from 1 to 2, but not back. They form separate Reaction Cycles.

## Input Format
- The first line contains two integers n and m: the number of substances and reactions.
- The following m lines describe the connections. Each line has two integers a and b, indicating a one-way reaction from substance a to substance b.

## Output Format
- Return one integer: the total number of Reaction Cycles.

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
