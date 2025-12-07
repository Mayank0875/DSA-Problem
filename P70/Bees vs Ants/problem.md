## Title
Bees vs Ants

## Slug
bees-vs-ants

## Difficulty
Medium

## Description
Bees fly between flowers. Ants crawl between flowers. Ants use paths where Bees don't have a direct flight line.

The garden has n flowers numbered from 1 to n.
The Flight Path connects specific pairs of flowers with direct flights.
The Crawl Path is constructed based on a unique rule:
A direct crawl exists between two flowers if and only if there is no flight connecting them.

Moving between any two connected flowers takes exactly 1 hour on either network.
Two insects, The Bee and The Ant, depart from flower 1 at the same time, heading for flower n.

1. The Bee travels only using Flight Path.
2. The Ant travels only using Crawl Path.

To ensure safety, they must never arrive at the same flower at the same time (except for the final flower n).
Your task is to compute the minimum number of hours required for **both** insects to reach flower n — specifically, the time when the slower insect arrives.
If either insect cannot reach flower n using their respective network, return -1.

## Examples

### 1

#### Input
4 2
1 3
3 4

#### Output
2

#### Explanation
The smallest possible time is 2. One takes the direct route (1 hour), the other takes a path of length 2.

### 2

#### Input
4 6
1 2
1 3
1 4
2 3
2 4
3 4

#### Output
-1

#### Explanation
The graph is fully connected for one network, meaning the complement network has no edges. The second insect cannot reach the destination.

## Input Format
- The first line contains two integers n and m, representing the number of flowers and the number of flights.
- The next m lines each contain two integers u and v, representing a flight between flowers u and v.
- The graph is bidirectional. There is at most one flight between any pair of flowers.

## Output Format
- Return a single integer representing the minimum hours required for the last insect to arrive. If it is impossible, return -1.

## Constraints
- 2 ≤ n ≤ 400
- 0 ≤ m ≤ n(n - 1)/2
- 1 ≤ u, v ≤ n
- u ≠ v

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph, breadth-first-search
