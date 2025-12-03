## Title
Political Alliances

## Slug
political-alliances

## Difficulty
Medium

## Description
Politicians endorse others. A Faction is a group where endorsements are mutual.

Two politicians a and b belong to the same Faction if and only if: It is possible to move from a to b, and it is also possible to move from b to a using the network of endorsements.
In other words, two politicians are in the same Faction if they are mutually reachable.

Your task is to: Determine how many Factions exist in total.

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
The politicians form two distinct groups where round-trip traversal is possible within each group.
Politicians {1, 2, 3} form one Faction.
Path: 1 -> 2 -> 3 -> 1.
Politicians {4, 5} form another Faction.
Path: 4 -> 5 -> 4.
Total Factions: 2.

### 2

#### Input
2 1
1 2

#### Output
2

#### Explanation
There are 2 politicians and 1 one-way endorsement.
Endorsement: 1 -> 2.
One can go from 1 to 2, but not back. They form separate Factions.

## Input Format
- The first line contains two integers n and m: the number of politicians and endorsements.
- The following m lines describe the connections. Each line has two integers a and b, indicating a one-way endorsement from politician a to politician b.

## Output Format
- Return one integer: the total number of Factions.

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
