## Title
Village Festival Decor

## Slug
village-festival-decor

## Difficulty
Medium

## Description
Houses in a village are connected by paths. Neighbors want to hang banners across the path between them. Each house can support one end of a banner.

The structure is a tree with n houses and n-1 paths.
A banner is formed between two houses connected by a path.
However, each house can be part of at most one banner.

Your task is to calculate the maximum number of banners that can be formed.

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
One optimal set of banners is (1, 2) and (3, 4). Node 5 remains unpaired. This gives a total of 2 banners.

### 2

#### Input
4
1 2
2 3
3 4

#### Output
2

#### Explanation
We can form banners (1, 2) and (3, 4), giving a total of 2.

## Input Format
- The first line contains an integer n, the number of houses.
- The next n-1 lines each contain two integers u and v, representing a path between house u and house v.

## Output Format
- Return a single integer representing the maximum number of banners.

## Constraints
- 1 ≤ n ≤ 2e5
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, graph
