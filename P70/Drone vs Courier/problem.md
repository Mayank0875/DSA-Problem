## Title
Drone vs Courier

## Slug
drone-vs-courier

## Difficulty
Medium

## Description
A Delivery Drone flies. A Bike Courier rides. Bikes take routes where Drones can't fly directly.

The delivery zone has n drop-offs numbered from 1 to n.
The Air Lane connects specific pairs of drop-offs with direct flights.
The Bike Lane is constructed based on a unique rule:
A direct ride exists between two drop-offs if and only if there is no flight connecting them.

Moving between any two connected drop-offs takes exactly 1 hour on either network.
Two deliverers, The Drone and The Biker, depart from drop-off 1 at the same time, heading for drop-off n.

1. The Drone travels only using Air Lane.
2. The Biker travels only using Bike Lane.

To ensure safety, they must never arrive at the same drop-off at the same time (except for the final drop-off n).
Your task is to compute the minimum number of hours required for **both** deliverers to reach drop-off n — specifically, the time when the slower deliverer arrives.
If either deliverer cannot reach drop-off n using their respective network, return -1.

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
The graph is fully connected for one network, meaning the complement network has no edges. The second deliverer cannot reach the destination.

## Input Format
- The first line contains two integers n and m, representing the number of drop-offs and the number of flights.
- The next m lines each contain two integers u and v, representing a flight between drop-offs u and v.
- The graph is bidirectional. There is at most one flight between any pair of drop-offs.

## Output Format
- Return a single integer representing the minimum hours required for the last deliverer to arrive. If it is impossible, return -1.

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
