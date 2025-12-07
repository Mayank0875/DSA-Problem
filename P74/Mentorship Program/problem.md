## Title
Mentorship Program

## Slug
mentorship-program

## Difficulty
Medium

## Description
A company organization chart is a tree. HR wants to create mentorship pairs where a manager mentors a direct report (or vice versa). Each employee can only be in one mentorship relationship.

The structure is a tree with n employees and n-1 reporting lines.
A mentorship pair is formed between two employees connected by a reporting line.
However, each employee can be part of at most one mentorship pair.

Your task is to calculate the maximum number of mentorship pairs that can be formed.

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
One optimal set of mentorship pairs is (1, 2) and (3, 4). Node 5 remains unpaired. This gives a total of 2 mentorship pairs.

### 2

#### Input
4
1 2
2 3
3 4

#### Output
2

#### Explanation
We can form mentorship pairs (1, 2) and (3, 4), giving a total of 2.

## Input Format
- The first line contains an integer n, the number of employees.
- The next n-1 lines each contain two integers u and v, representing a reporting line between employee u and employee v.

## Output Format
- Return a single integer representing the maximum number of mentorship pairs.

## Constraints
- 1 ≤ n ≤ 2e5
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, graph
