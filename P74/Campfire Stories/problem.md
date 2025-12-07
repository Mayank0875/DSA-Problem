## Title
Campfire Stories

## Slug
campfire-stories

## Difficulty
Medium

## Description
Campers sit in a non-circular arrangement (tree). Adjacent campers share a blanket. Each camper shares with one person.

The structure is a tree with n campers and n-1 positions.
A blanket share is formed between two campers connected by a position.
However, each camper can be part of at most one blanket share.

Your task is to calculate the maximum number of blanket shares that can be formed.

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
One optimal set of blanket shares is (1, 2) and (3, 4). Node 5 remains unpaired. This gives a total of 2 blanket shares.

### 2

#### Input
4
1 2
2 3
3 4

#### Output
2

#### Explanation
We can form blanket shares (1, 2) and (3, 4), giving a total of 2.

## Input Format
- The first line contains an integer n, the number of campers.
- The next n-1 lines each contain two integers u and v, representing a position between camper u and camper v.

## Output Format
- Return a single integer representing the maximum number of blanket shares.

## Constraints
- 1 ≤ n ≤ 2e5
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, graph
