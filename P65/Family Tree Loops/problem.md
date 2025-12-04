## Title
Family Tree Loops

## Slug
family-tree-loops

## Difficulty
Medium

## Description
Due to time travel, ancestors can descend from descendants. A Paradox Clan is a group related cyclically.

Two people a and b belong to the same Clan if and only if: It is possible to move from a to b, and it is also possible to move from b to a using the network of lineages.
In other words, two people are in the same Clan if they are mutually reachable.

Your task is to: Determine how many Clans exist in total.

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
The people form two distinct groups where round-trip traversal is possible within each group.
People {1, 2, 3} form one Clan.
Path: 1 -> 2 -> 3 -> 1.
People {4, 5} form another Clan.
Path: 4 -> 5 -> 4.
Total Clans: 2.

### 2

#### Input
2 1
1 2

#### Output
2

#### Explanation
There are 2 people and 1 one-way lineage.
Lineage: 1 -> 2.
One can go from 1 to 2, but not back. They form separate Clans.

## Input Format
- The first line contains two integers n and m: the number of people and lineages.
- The following m lines describe the connections. Each line has two integers a and b, indicating a one-way lineage from person a to person b.

## Output Format
- Return one integer: the total number of Clans.

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
