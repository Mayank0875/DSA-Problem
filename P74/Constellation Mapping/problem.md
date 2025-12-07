## Title
Constellation Mapping

## Slug
constellation-mapping

## Difficulty
Medium

## Description
Stars in a constellation are linked by imaginary lines. Astronomers want to name binary pairs of connected stars. Each star can belong to one named binary.

The structure is a tree with n stars and n-1 lines.
A binary system is formed between two stars connected by a line.
However, each star can be part of at most one binary system.

Your task is to calculate the maximum number of binary systems that can be formed.

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
One optimal set of binary systems is (1, 2) and (3, 4). Node 5 remains unpaired. This gives a total of 2 binary systems.

### 2

#### Input
4
1 2
2 3
3 4

#### Output
2

#### Explanation
We can form binary systems (1, 2) and (3, 4), giving a total of 2.

## Input Format
- The first line contains an integer n, the number of stars.
- The next n-1 lines each contain two integers u and v, representing a line between star u and star v.

## Output Format
- Return a single integer representing the maximum number of binary systems.

## Constraints
- 1 ≤ n ≤ 2e5
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, graph
