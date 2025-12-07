## Title
Genealogy DNA Test

## Slug
genealogy-dna-test

## Difficulty
Medium

## Description
A family tree is being studied. Researchers want to compare DNA between direct relatives (parent-child). Each person can be part of only one comparison.

The structure is a tree with n relatives and n-1 relations.
A comparison is formed between two relatives connected by a relation.
However, each relative can be part of at most one comparison.

Your task is to calculate the maximum number of comparisons that can be formed.

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
One optimal set of comparisons is (1, 2) and (3, 4). Node 5 remains unpaired. This gives a total of 2 comparisons.

### 2

#### Input
4
1 2
2 3
3 4

#### Output
2

#### Explanation
We can form comparisons (1, 2) and (3, 4), giving a total of 2.

## Input Format
- The first line contains an integer n, the number of relatives.
- The next n-1 lines each contain two integers u and v, representing a relation between relative u and relative v.

## Output Format
- Return a single integer representing the maximum number of comparisons.

## Constraints
- 1 ≤ n ≤ 2e5
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, graph
