## Title
Office Desk Arrangement

## Slug
office-desk-arrangement

## Difficulty
Medium

## Description
Desks are arranged in clusters. Managers pair up adjacent desks for pair programming. Each desk is part of one pair.

The structure is a tree with n desks and n-1 proximity.
A pair programming team is formed between two desks connected by a proximity.
However, each desk can be part of at most one pair programming team.

Your task is to calculate the maximum number of pair programming teams that can be formed.

## Examples

### 1

#### Input
5
1 2
1 3
3 4
3 5

#### Output
2

#### Explanation
One optimal set of pair programming teams is (1, 2) and (3, 4). Node 5 remains unpaired. This gives a total of 2 pair programming teams.

### 2

#### Input
4
1 2
2 3
3 4

#### Output
2

#### Explanation
We can form pair programming teams (1, 2) and (3, 4), giving a total of 2.

## Input Format
- The first line contains an integer n, the number of desks.
- The next n-1 lines each contain two integers u and v, representing a proximity between desk u and desk v.

## Output Format
- Return a single integer representing the maximum number of pair programming teams.

## Constraints
- 1 ≤ n ≤ 2e5
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, graph
