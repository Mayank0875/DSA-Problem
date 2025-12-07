## Title
Ballroom Dance Partners

## Slug
ballroom-dance-partners

## Difficulty
Medium

## Description
A dance instructor is pairing students for a ballroom competition. The students are arranged in a formation where friendships link them in a tree structure. To ensure chemistry, partners must be friends (connected).

The structure is a tree with n students and n-1 friendships.
A pair is formed between two students connected by a friendship.
However, each student can be part of at most one pair.

Your task is to calculate the maximum number of pairs that can be formed.

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
One optimal set of pairs is (1, 2) and (3, 4). Node 5 remains unpaired. This gives a total of 2 pairs.

### 2

#### Input
4
1 2
2 3
3 4

#### Output
2

#### Explanation
We can form pairs (1, 2) and (3, 4), giving a total of 2.

## Input Format
- The first line contains an integer n, the number of students.
- The next n-1 lines each contain two integers u and v, representing a friendship between student u and student v.

## Output Format
- Return a single integer representing the maximum number of pairs.

## Constraints
- 1 ≤ n ≤ 2e5
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, graph
