## Title
Fashion Show Models

## Slug
fashion-show-models

## Difficulty
Medium

## Description
Models are waiting backstage in a tree layout of rooms. They walk the runway in pairs from adjacent rooms.

The structure is a tree with n models and n-1 doorways.
A runway pair is formed between two models connected by a doorway.
However, each model can be part of at most one runway pair.

Your task is to calculate the maximum number of runway pairs that can be formed.

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
One optimal set of runway pairs is (1, 2) and (3, 4). Node 5 remains unpaired. This gives a total of 2 runway pairs.

### 2

#### Input
4
1 2
2 3
3 4

#### Output
2

#### Explanation
We can form runway pairs (1, 2) and (3, 4), giving a total of 2.

## Input Format
- The first line contains an integer n, the number of models.
- The next n-1 lines each contain two integers u and v, representing a doorway between model u and model v.

## Output Format
- Return a single integer representing the maximum number of runway pairs.

## Constraints
- 1 ≤ n ≤ 2e5
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, graph
