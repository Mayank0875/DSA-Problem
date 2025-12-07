## Title
University Department Grants

## Slug
university-department-grants

## Difficulty
Medium

## Description
Departments collaborate on grants. Adjacent departments in the building apply together. Each department applies for one joint grant.

The structure is a tree with n departments and n-1 hallways.
A grant application is formed between two departments connected by a hallway.
However, each department can be part of at most one grant application.

Your task is to calculate the maximum number of grant applications that can be formed.

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
One optimal set of grant applications is (1, 2) and (3, 4). Node 5 remains unpaired. This gives a total of 2 grant applications.

### 2

#### Input
4
1 2
2 3
3 4

#### Output
2

#### Explanation
We can form grant applications (1, 2) and (3, 4), giving a total of 2.

## Input Format
- The first line contains an integer n, the number of departments.
- The next n-1 lines each contain two integers u and v, representing a hallway between department u and department v.

## Output Format
- Return a single integer representing the maximum number of grant applications.

## Constraints
- 1 ≤ n ≤ 2e5
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, graph
