## Title
Bird Nesting Pairs

## Slug
bird-nesting-pairs

## Difficulty
Medium

## Description
Birds have built nests in a large tree structure. During mating season, birds from adjacent nests pair up. Each nest houses one bird.

The structure is a tree with n nests and n-1 branches.
A breeding pair is formed between two nests connected by a branch.
However, each nest can be part of at most one breeding pair.

Your task is to calculate the maximum number of breeding pairs that can be formed.

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
One optimal set of breeding pairs is (1, 2) and (3, 4). Node 5 remains unpaired. This gives a total of 2 breeding pairs.

### 2

#### Input
4
1 2
2 3
3 4

#### Output
2

#### Explanation
We can form breeding pairs (1, 2) and (3, 4), giving a total of 2.

## Input Format
- The first line contains an integer n, the number of nests.
- The next n-1 lines each contain two integers u and v, representing a branch between nest u and nest v.

## Output Format
- Return a single integer representing the maximum number of breeding pairs.

## Constraints
- 1 ≤ n ≤ 2e5
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, graph
