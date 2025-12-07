## Title
Restaurant Table Joining

## Slug
restaurant-table-joining

## Difficulty
Medium

## Description
Tables are arranged in a layout. Waiters push adjacent tables together for large parties. Each table can be joined to one other.

The structure is a tree with n tables and n-1 spaces.
A large table is formed between two tables connected by a space.
However, each table can be part of at most one large table.

Your task is to calculate the maximum number of large tables that can be formed.

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
One optimal set of large tables is (1, 2) and (3, 4). Node 5 remains unpaired. This gives a total of 2 large tables.

### 2

#### Input
4
1 2
2 3
3 4

#### Output
2

#### Explanation
We can form large tables (1, 2) and (3, 4), giving a total of 2.

## Input Format
- The first line contains an integer n, the number of tables.
- The next n-1 lines each contain two integers u and v, representing a space between table u and table v.

## Output Format
- Return a single integer representing the maximum number of large tables.

## Constraints
- 1 ≤ n ≤ 2e5
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, graph
