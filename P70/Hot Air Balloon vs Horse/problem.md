## Title
Hot Air Balloon vs Horse

## Slug
hot-air-balloon-vs-horse

## Difficulty
Medium

## Description
A Balloonist flies. A Rider gallops. The Rider takes roads where the Balloon cannot catch the wind.

The plains has n towns numbered from 1 to n.
The Wind Route connects specific pairs of towns with direct drafts.
The Dirt Road is constructed based on a unique rule:
A direct track exists between two towns if and only if there is no draft connecting them.

Moving between any two connected towns takes exactly 1 hour on either network.
Two racers, The Balloonist and The Rider, depart from town 1 at the same time, heading for town n.

1. The Balloonist travels only using Wind Route.
2. The Rider travels only using Dirt Road.

To ensure safety, they must never arrive at the same town at the same time (except for the final town n).
Your task is to compute the minimum number of hours required for **both** racers to reach town n — specifically, the time when the slower racer arrives.
If either racer cannot reach town n using their respective network, return -1.

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
The graph is fully connected for one network, meaning the complement network has no edges. The second racer cannot reach the destination.

## Input Format
- The first line contains two integers n and m, representing the number of towns and the number of drafts.
- The next m lines each contain two integers u and v, representing a draft between towns u and v.
- The graph is bidirectional. There is at most one draft between any pair of towns.

## Output Format
- Return a single integer representing the minimum hours required for the last racer to arrive. If it is impossible, return -1.

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
