## Title
Coral Reef Polyps

## Slug
coral-reef-polyps

## Difficulty
Medium

## Description
Polyps on a coral branch are connected. They share nutrients in pairs. Each polyp can share with only one neighbor.

The structure is a tree with n polyps and n-1 structures.
A nutrient link is formed between two polyps connected by a structure.
However, each polyp can be part of at most one nutrient link.

Your task is to calculate the maximum number of nutrient links that can be formed.

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
One optimal set of nutrient links is (1, 2) and (3, 4). Node 5 remains unpaired. This gives a total of 2 nutrient links.

### 2

#### Input
4
1 2
2 3
3 4

#### Output
2

#### Explanation
We can form nutrient links (1, 2) and (3, 4), giving a total of 2.

## Input Format
- The first line contains an integer n, the number of polyps.
- The next n-1 lines each contain two integers u and v, representing a structure between polyp u and polyp v.

## Output Format
- Return a single integer representing the maximum number of nutrient links.

## Constraints
- 1 ≤ n ≤ 2e5
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, graph
