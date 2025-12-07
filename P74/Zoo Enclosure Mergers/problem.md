## Title
Zoo Enclosure Mergers

## Slug
zoo-enclosure-mergers

## Difficulty
Medium

## Description
Animal enclosures are adjacent. The zoo wants to remove fences between pairs of enclosures to make larger habitats. Each enclosure joins one neighbor.

The structure is a tree with n enclosures and n-1 fences.
A habitat is formed between two enclosures connected by a fence.
However, each enclosure can be part of at most one habitat.

Your task is to calculate the maximum number of habitats that can be formed.

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
One optimal set of habitats is (1, 2) and (3, 4). Node 5 remains unpaired. This gives a total of 2 habitats.

### 2

#### Input
4
1 2
2 3
3 4

#### Output
2

#### Explanation
We can form habitats (1, 2) and (3, 4), giving a total of 2.

## Input Format
- The first line contains an integer n, the number of enclosures.
- The next n-1 lines each contain two integers u and v, representing a fence between enclosure u and enclosure v.

## Output Format
- Return a single integer representing the maximum number of habitats.

## Constraints
- 1 ≤ n ≤ 2e5
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, graph
