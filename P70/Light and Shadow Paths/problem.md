## Title
Light and Shadow Paths

## Slug
light-and-shadow-paths

## Difficulty
Medium

## Description
Two spirits traverse the Spirit World. The Light Spirit uses Sun Beams, and the Shadow Spirit uses Shadow Steps. A Shadow Step exists between two nodes only if a Sun Beam does not.

The spirit world has n shrines numbered from 1 to n.
The Light Web connects specific pairs of shrines with direct sun beams.
The Shadow Web is constructed based on a unique rule:
A direct shadow step exists between two shrines if and only if there is no sun beam connecting them.

Moving between any two connected shrines takes exactly 1 hour on either network.
Two spirits, The Light Spirit and The Shadow Spirit, depart from shrine 1 at the same time, heading for shrine n.

1. The Light Spirit travels only using Light Web.
2. The Shadow Spirit travels only using Shadow Web.

To ensure safety, they must never arrive at the same shrine at the same time (except for the final shrine n).
Your task is to compute the minimum number of hours required for **both** spirits to reach shrine n — specifically, the time when the slower spirit arrives.
If either spirit cannot reach shrine n using their respective network, return -1.

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
The graph is fully connected for one network, meaning the complement network has no edges. The second spirit cannot reach the destination.

## Input Format
- The first line contains two integers n and m, representing the number of shrines and the number of sun beams.
- The next m lines each contain two integers u and v, representing a sun beam between shrines u and v.
- The graph is bidirectional. There is at most one sun beam between any pair of shrines.

## Output Format
- Return a single integer representing the minimum hours required for the last spirit to arrive. If it is impossible, return -1.

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
