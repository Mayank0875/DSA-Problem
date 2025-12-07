## Title
Study Buddies

## Slug
study-buddies

## Difficulty
Medium

## Description
Students sit in a classroom arrangement shaped like a tree graph. The teacher asks them to form study pairs with a neighbor they are directly connected to.

The structure is a tree with n students and n-1 aisles.
A study pair is formed between two students connected by a aisle.
However, each student can be part of at most one study pair.

Your task is to calculate the maximum number of study pairs that can be formed.

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
One optimal set of study pairs is (1, 2) and (3, 4). Node 5 remains unpaired. This gives a total of 2 study pairs.

### 2

#### Input
4
1 2
2 3
3 4

#### Output
2

#### Explanation
We can form study pairs (1, 2) and (3, 4), giving a total of 2.

## Input Format
- The first line contains an integer n, the number of students.
- The next n-1 lines each contain two integers u and v, representing a aisle between student u and student v.

## Output Format
- Return a single integer representing the maximum number of study pairs.

## Constraints
- 1 ≤ n ≤ 2e5
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, graph
