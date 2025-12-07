## Title
Online vs Offline

## Slug
online-vs-offline

## Difficulty
Medium

## Description
Information spreads through a group. Online Messages go through the internet. Offline Whispers go between people who aren't connected online.

The social graph has n people numbered from 1 to n.
The Online Web connects specific pairs of people with direct connections.
The Offline Web is constructed based on a unique rule:
A direct whisper exists between two people if and only if there is no connection connecting them.

Moving between any two connected people takes exactly 1 hour on either network.
Two messages, The Email and The Rumor, depart from person 1 at the same time, heading for person n.

1. The Email travels only using Online Web.
2. The Rumor travels only using Offline Web.

To ensure safety, they must never arrive at the same person at the same time (except for the final person n).
Your task is to compute the minimum number of hours required for **both** messages to reach person n — specifically, the time when the slower message arrives.
If either message cannot reach person n using their respective network, return -1.

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
The graph is fully connected for one network, meaning the complement network has no edges. The second message cannot reach the destination.

## Input Format
- The first line contains two integers n and m, representing the number of people and the number of connections.
- The next m lines each contain two integers u and v, representing a connection between people u and v.
- The graph is bidirectional. There is at most one connection between any pair of people.

## Output Format
- Return a single integer representing the minimum hours required for the last message to arrive. If it is impossible, return -1.

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
