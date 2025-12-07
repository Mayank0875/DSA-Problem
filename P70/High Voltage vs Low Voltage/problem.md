## Title
High Voltage vs Low Voltage

## Slug
high-voltage-vs-low-voltage

## Difficulty
Medium

## Description
High Voltage current uses Power Lines. Low Voltage control signals use Data Cables. Data Cables connect substations not linked by Power Lines.

The grid has n substations numbered from 1 to n.
The HV Grid connects specific pairs of substations with direct power lines.
The LV Grid is constructed based on a unique rule:
A direct data cable exists between two substations if and only if there is no power line connecting them.

Moving between any two connected substations takes exactly 1 hour on either network.
Two currents, High Voltage and Low Voltage, depart from substation 1 at the same time, heading for substation n.

1. High Voltage travels only using HV Grid.
2. Low Voltage travels only using LV Grid.

To ensure safety, they must never arrive at the same substation at the same time (except for the final substation n).
Your task is to compute the minimum number of hours required for **both** currents to reach substation n — specifically, the time when the slower current arrives.
If either current cannot reach substation n using their respective network, return -1.

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
The graph is fully connected for one network, meaning the complement network has no edges. The second current cannot reach the destination.

## Input Format
- The first line contains two integers n and m, representing the number of substations and the number of power lines.
- The next m lines each contain two integers u and v, representing a power line between substations u and v.
- The graph is bidirectional. There is at most one power line between any pair of substations.

## Output Format
- Return a single integer representing the minimum hours required for the last current to arrive. If it is impossible, return -1.

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
