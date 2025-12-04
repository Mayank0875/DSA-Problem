## Title
Ant Colony Chambers

## Slug
ant-colony-chambers

## Difficulty
Medium

## Description
An ant hill has N chambers linked by one-way tunnels. A Nest Section is a group of chambers fully accessible from each other.

Two chambers a and b belong to the same Nest Section if and only if: It is possible to move from a to b, and it is also possible to move from b to a using the network of tunnels.
In other words, two chambers are in the same Nest Section if they are mutually reachable.

Your task is to: Determine how many Nest Sections exist in total.

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
The chambers form two distinct groups where round-trip traversal is possible within each group.
Chambers {1, 2, 3} form one Nest Section.
Path: 1 -> 2 -> 3 -> 1.
Chambers {4, 5} form another Nest Section.
Path: 4 -> 5 -> 4.
Total Nest Sections: 2.

### 2

#### Input
2 1
1 2

#### Output
2

#### Explanation
There are 2 chambers and 1 one-way tunnel.
Tunnel: 1 -> 2.
One can go from 1 to 2, but not back. They form separate Nest Sections.

## Input Format
- The first line contains two integers n and m: the number of chambers and tunnels.
- The following m lines describe the connections. Each line has two integers a and b, indicating a one-way tunnel from chamber a to chamber b.

## Output Format
- Return one integer: the total number of Nest Sections.

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
