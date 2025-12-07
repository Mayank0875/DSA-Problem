## Title
Troop Reinforcements

## Slug
troop-reinforcements

## Difficulty
Hard

## Description
Soldiers need to move from the barracks to the front line. The bridges and paths can only support a certain number of troops marching at once.

The network consists of n outposts, numbered 1 to n.
1. Outpost 1 is the Barracks.
2. Outpost n is the Front Line.

There are m one-way paths connecting these outposts. Each path has a specific capacity, measured in soldiers per hour, which limits the rate at which troops can flow through it.

Multiple paths can exist between the same two outposts, and their capacities stack. Your goal is to determine the maximum total reinforcement rate that can be achieved from the Barracks to the Front Line using the available network.

## Examples

### 1

#### Input
4 5
1 2 3
2 4 2
1 3 4
3 4 5
4 1 3

#### Output
6

#### Explanation
There are two main paths to transmit troops from node 1 to node 4:
1 -> 2 -> 4 (capacity limited by link 2 -> 4 with capacity 2).
1 -> 3 -> 4 (capacity limited by link 1 -> 3 with capacity 4).
Total max flow is 2 + 4 = 6. The link 4 -> 1 is ignored because it flows backward from the destination.

### 2

#### Input
3 2
1 2 5
2 3 5

#### Output
5

#### Explanation
A single path 1 -> 2 -> 3 exists with a bottleneck capacity of 5.

## Input Format
- The first line contains two integers n and m: the number of outposts and the number of paths.
- The next m lines describe the paths. Each line contains three integers u, v, and c, indicating a one-way path from Outpost u to Outpost v with capacity c.

## Output Format
- Return one integer: the maximum reinforcement rate from Outpost 1 to Outpost n.

## Constraints
- 1 ≤ n ≤ 500
- 1 ≤ m ≤ 1000
- 1 ≤ u, v ≤ n
- 1 ≤ c ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph
