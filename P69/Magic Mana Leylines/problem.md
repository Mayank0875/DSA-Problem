## Title
Magic Mana Leylines

## Slug
magic-mana-leylines

## Difficulty
Hard

## Description
A wizard draws mana from a source crystal to cast a spell at a target location. The leylines connecting power nodes have capacity limits.

The network consists of n nodes, numbered 1 to n.
1. Mana Node 1 is the Source Crystal.
2. Mana Node n is the Spell Circle.

There are m one-way leylines connecting these nodes. Each leyline has a specific capacity, measured in mana points per second, which limits the rate at which mana can flow through it.

Multiple leylines can exist between the same two nodes, and their capacities stack. Your goal is to determine the maximum total magic power that can be achieved from the Source Crystal to the Spell Circle using the available network.

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
There are two main paths to transmit mana from node 1 to node 4:
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
- The first line contains two integers n and m: the number of nodes and the number of leylines.
- The next m lines describe the leylines. Each line contains three integers u, v, and c, indicating a one-way leyline from Mana Node u to Mana Node v with capacity c.

## Output Format
- Return one integer: the maximum magic power from Mana Node 1 to Mana Node n.

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
