## Title

The Dual Transport Race

## Slug

the-dual-transport-race

## Difficulty

Medium

## Description

In the futuristic city of Neotopia, travel is managed by two competing networks: the high-speed Hyperloop and the vintage Asphalt Roads. The city has n stations numbered from 1 to n.
The Hyperloop connects specific pairs of stations with direct tracks.
The Asphalt network is constructed based on a unique rule:
A direct road exists between two stations if and only if there is no Hyperloop track connecting them.

Traveling between any two connected stations takes exactly 1 hour on either network.
Two couriers, Red and Blue, depart from station 1 at the same time, heading for station n.

    1. Red travels only using Hyperloop tracks.
    2. Blue travels only using Asphalt Roads.

To ensure safety, they must never arrive at the same station at the same time (except for the final station n).
Your task:
Compute the minimum number of hours required for both couriers to reach station n — meaning the time when the slower courier arrives.
If either courier cannot reach station n using their respective network, return -1.

## Examples

### 1

#### Input

4 2
1 3
3 4


#### Output

2

#### Explanation

The smallest possible time is 2.
    
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

There are no roads, so there's no way for the bus to reach town 4.  

## Input Format  

- The first line contains two integers n and m, representing the number of stations and the number of Hyperloop tracks.
- The next m lines each contain two integers u and v, representing a Hyperloop track between stations u and v.
- The graph is bidirectional. There is at most one track between any pair of stations.

## Output Format  

- Return a single integer representing the minimum hours required for the last courier to arrive. If it is impossible, return -1.  

## Constraints  

- 2 ≤ n ≤ 400
- 0 ≤ m ≤ n(n - 1)/2
- 1 ≤ u, v ≤ n
- u ≠ v


## Time Limit

2 second

## Memory Limit

256 MB

## Tags

graph, depth-first-search, hackwithinfy

## Companies
infosys