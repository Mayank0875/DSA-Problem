## Title
Internet Routing Peers

## Slug
internet-routing-peers

## Difficulty
Medium

## Description
Autonomous Systems (AS) route traffic. A Peering Group is a set of AS that can route traffic to each other cyclically.

Two systems a and b belong to the same Peering Group if and only if: It is possible to move from a to b, and it is also possible to move from b to a using the network of links.
In other words, two systems are in the same Peering Group if they are mutually reachable.

Your task is to: Determine how many Peering Groups exist in total.

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
The systems form two distinct groups where round-trip traversal is possible within each group.
Systems {1, 2, 3} form one Peering Group.
Path: 1 -> 2 -> 3 -> 1.
Systems {4, 5} form another Peering Group.
Path: 4 -> 5 -> 4.
Total Peering Groups: 2.

### 2

#### Input
2 1
1 2

#### Output
2

#### Explanation
There are 2 systems and 1 one-way link.
Link: 1 -> 2.
One can go from 1 to 2, but not back. They form separate Peering Groups.

## Input Format
- The first line contains two integers n and m: the number of systems and links.
- The following m lines describe the connections. Each line has two integers a and b, indicating a one-way link from system a to system b.

## Output Format
- Return one integer: the total number of Peering Groups.

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
