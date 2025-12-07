## Title
Hovercar vs Maglev

## Slug
hovercar-vs-maglev

## Difficulty
Medium

## Description
Hovercars use air lanes. Maglevs use rails. Rails connect stations not served by air lanes.

The metropolis has n stops numbered from 1 to n.
The Air Traffic connects specific pairs of stops with direct lanes.
The Rail Traffic is constructed based on a unique rule:
A direct track exists between two stops if and only if there is no lane connecting them.

Moving between any two connected stops takes exactly 1 hour on either network.
Two commuters, The Pilot and The Passenger, depart from stop 1 at the same time, heading for stop n.

1. The Pilot travels only using Air Traffic.
2. The Passenger travels only using Rail Traffic.

To ensure safety, they must never arrive at the same stop at the same time (except for the final stop n).
Your task is to compute the minimum number of hours required for **both** commuters to reach stop n — specifically, the time when the slower commuter arrives.
If either commuter cannot reach stop n using their respective network, return -1.

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
The graph is fully connected for one network, meaning the complement network has no edges. The second commuter cannot reach the destination.

## Input Format
- The first line contains two integers n and m, representing the number of stops and the number of lanes.
- The next m lines each contain two integers u and v, representing a lane between stops u and v.
- The graph is bidirectional. There is at most one lane between any pair of stops.

## Output Format
- Return a single integer representing the minimum hours required for the last commuter to arrive. If it is impossible, return -1.

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
