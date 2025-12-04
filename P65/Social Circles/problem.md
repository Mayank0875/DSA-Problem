## Title
Social Circles

## Slug
social-circles

## Difficulty
Medium

## Description
In a social network, N people have directed relationships (A trusts B). A Social Circle is a group where everyone trusts everyone else, directly or indirectly (trust is mutual and transitive).

Two people a and b belong to the same Social Circle if and only if: It is possible to move from a to b, and it is also possible to move from b to a using the network of trust links.
In other words, two people are in the same Social Circle if they are mutually reachable.

Your task is to: Determine how many Social Circles exist in total.

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
The people form two distinct groups where round-trip traversal is possible within each group.
People {1, 2, 3} form one Social Circle.
Path: 1 -> 2 -> 3 -> 1.
People {4, 5} form another Social Circle.
Path: 4 -> 5 -> 4.
Total Social Circles: 2.

### 2

#### Input
2 1
1 2

#### Output
2

#### Explanation
There are 2 people and 1 one-way trust link.
Trust link: 1 -> 2.
One can go from 1 to 2, but not back. They form separate Social Circles.

## Input Format
- The first line contains two integers n and m: the number of people and trust links.
- The following m lines describe the connections. Each line has two integers a and b, indicating a one-way trust link from person a to person b.

## Output Format
- Return one integer: the total number of Social Circles.

## Constraints
- 1 ≤ n ≤ 1e5
- 1 ≤ m ≤ 2e5
- 1 ≤ a, b ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph, depth-first-search
