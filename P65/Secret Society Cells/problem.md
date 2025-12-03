## Title
Secret Society Cells

## Slug
secret-society-cells

## Difficulty
Medium

## Description
Members of a secret society know the identity of other members in a directed chain. A Cell is a group where information can flow between all members.

Two members a and b belong to the same Cell if and only if: It is possible to move from a to b, and it is also possible to move from b to a using the network of contacts.
In other words, two members are in the same Cell if they are mutually reachable.

Your task is to: Determine how many Cells exist in total.

## Examples

### 1

#### Input
5 6
1 2
2 3
3 1
3 4
4 5
5 4

#### Output
2

#### Explanation
The members form two distinct groups where round-trip traversal is possible within each group.
Members {1, 2, 3} form one Cell.
Path: 1 -> 2 -> 3 -> 1.
Members {4, 5} form another Cell.
Path: 4 -> 5 -> 4.
Total Cells: 2.

### 2

#### Input
2 1
1 2

#### Output
2

#### Explanation
There are 2 members and 1 one-way contact.
Contact: 1 -> 2.
One can go from 1 to 2, but not back. They form separate Cells.

## Input Format
- The first line contains two integers n and m: the number of members and contacts.
- The following m lines describe the connections. Each line has two integers a and b, indicating a one-way contact from member a to member b.

## Output Format
- Return one integer: the total number of Cells.

## Constraints
- 1 ≤ n ≤ 1e5
- 1 ≤ m ≤ 2e5
- 1 ≤ a, b ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph, depth-first-search, strongly-connected-components
