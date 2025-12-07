## Title
Distributed Computing

## Slug
distributed-computing

## Difficulty
Hard

## Description
A master node sends computation tasks to worker nodes. The network links restrict how many tasks can be sent.

The network consists of n switches, numbered 1 to n.
1. Switch 1 is the Master Node.
2. Switch n is the Worker Cluster.

There are m one-way cables connecting these switches. Each cable has a specific capacity, measured in jobs per second, which limits the rate at which tasks can flow through it.

Multiple cables can exist between the same two switches, and their capacities stack. Your goal is to determine the maximum total processing load that can be achieved from the Master Node to the Worker Cluster using the available network.

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
There are two main paths to transmit tasks from node 1 to node 4:
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
- The first line contains two integers n and m: the number of switches and the number of cables.
- The next m lines describe the cables. Each line contains three integers u, v, and c, indicating a one-way cable from Switch u to Switch v with capacity c.

## Output Format
- Return one integer: the maximum processing load from Switch 1 to Switch n.

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
