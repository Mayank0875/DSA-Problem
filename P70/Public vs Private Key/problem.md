## Title
Public vs Private Key

## Slug
public-vs-private-key

## Difficulty
Medium

## Description
Public data flows through Open Channels. Private data flows through Encrypted Tunnels. Tunnels link servers not linked by Open Channels.

The cloud has n servers numbered from 1 to n.
The Public Net connects specific pairs of servers with direct channels.
The Private Net is constructed based on a unique rule:
A direct tunnel exists between two servers if and only if there is no channel connecting them.

Moving between any two connected servers takes exactly 1 hour on either network.
Two data streams, Public Data and Private Data, depart from server 1 at the same time, heading for server n.

1. Public Data travels only using Public Net.
2. Private Data travels only using Private Net.

To ensure safety, they must never arrive at the same server at the same time (except for the final server n).
Your task is to compute the minimum number of hours required for **both** data streams to reach server n — specifically, the time when the slower data stream arrives.
If either data stream cannot reach server n using their respective network, return -1.

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
The graph is fully connected for one network, meaning the complement network has no edges. The second data stream cannot reach the destination.

## Input Format
- The first line contains two integers n and m, representing the number of servers and the number of channels.
- The next m lines each contain two integers u and v, representing a channel between servers u and v.
- The graph is bidirectional. There is at most one channel between any pair of servers.

## Output Format
- Return a single integer representing the minimum hours required for the last data stream to arrive. If it is impossible, return -1.

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
