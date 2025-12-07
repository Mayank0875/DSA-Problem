## Title
Summer vs Winter Roads

## Slug
summer-vs-winter-roads

## Difficulty
Medium

## Description
Logistics planners simulate routes. Summer Trucks use dirt roads. Winter Sleds use ice roads over frozen lakes, which exist where dirt roads don't.

The region has n outposts numbered from 1 to n.
The Summer Grid connects specific pairs of outposts with direct dirt roads.
The Winter Grid is constructed based on a unique rule:
A direct ice road exists between two outposts if and only if there is no dirt road connecting them.

Moving between any two connected outposts takes exactly 1 hour on either network.
Two vehicles, The Truck and The Sled, depart from outpost 1 at the same time, heading for outpost n.

1. The Truck travels only using Summer Grid.
2. The Sled travels only using Winter Grid.

To ensure safety, they must never arrive at the same outpost at the same time (except for the final outpost n).
Your task is to compute the minimum number of hours required for **both** vehicles to reach outpost n — specifically, the time when the slower vehicle arrives.
If either vehicle cannot reach outpost n using their respective network, return -1.

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
The graph is fully connected for one network, meaning the complement network has no edges. The second vehicle cannot reach the destination.

## Input Format
- The first line contains two integers n and m, representing the number of outposts and the number of dirt roads.
- The next m lines each contain two integers u and v, representing a dirt road between outposts u and v.
- The graph is bidirectional. There is at most one dirt road between any pair of outposts.

## Output Format
- Return a single integer representing the minimum hours required for the last vehicle to arrive. If it is impossible, return -1.

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
