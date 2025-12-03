## Title
Pipeline Redundancy

## Slug
pipeline-redundancy

## Difficulty
Medium

## Description
Two parallel oil pipelines need crossover valves to route flow around blockages.

Two parallel pipelines, Main Line and Auxiliary Line, each contain n pumping stations arranged in a line.
Main Line has an array `a` representing the pressure rating of each station.
Auxiliary Line has an array `b` representing the pressure rating of each station.

Inside each pipeline, adjacent pumping stations are already connected by internal pipes.

You must establish inter-pipeline crossover valves connecting some pumping stations of Main Line to some pumping stations of Auxiliary Line.

The cost to create a valve between station i of Main Line and station j of Auxiliary Line is:
absolute value of (a[i] - b[j]).

**Fault-tolerance requirement:**
The final network must remain fully connected even if any single station is removed (from either Main Line or Auxiliary Line).
If one station fails and disappears along with all its connections, the remaining pumping stations must still form a single connected network.

Your task is to calculate the minimum total cost required to build such a set of connections.

## Examples

### 1

#### Input
3
1 10 1
20 4 25

#### Output
31

#### Explanation
It's optimal to connect four pairs of pumping stations:
1. station 1 from Main Line with station 2 from Auxiliary Line: cost |1-4| = 3.
2. station 3 from Main Line with station 2 from Auxiliary Line: cost |1-4| = 3.
3. station 2 from Main Line with station 1 from Auxiliary Line: cost |10-20| = 10.
4. station 2 from Main Line with station 3 from Auxiliary Line: cost |10-25| = 15.
Total cost: 3 + 3 + 10 + 15 = 31.

### 2

#### Input
4
1 1 1 1
1000000000 1000000000 1000000000 1000000000

#### Output
1999999998

#### Explanation
It is optimal to connect the first station of Main Line with the first of Auxiliary Line, and the last station of Main Line with the last of Auxiliary Line, satisfying the connectivity conditions efficiently given the values.

## Input Format
- The first line contains an integer n, the number of pumping stations in each pipeline.
- The second line contains n integers representing the pressure ratings of Main Line.
- The third line contains n integers representing the pressure ratings of Auxiliary Line.

## Output Format
- Return a single integer representing the minimum total cost to make the network fault-tolerant.

## Constraints
- 3 ≤ n ≤ 10^5
- 1 ≤ a[i], b[i] ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph, greedy, math
