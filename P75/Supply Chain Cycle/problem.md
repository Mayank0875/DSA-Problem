## Title
Supply Chain Cycle

## Slug
supply-chain-cycle

## Difficulty
Medium

## Description
A logistics firm is auditing its supply chain. A circular dependency happens when a product's components eventually depend on the product itself.

A "cycle" occurs when a material moves from a factory, through a sequence of transport routes, and returns to the starting factory without traversing the same transport route twice in immediate succession. The "length" of such a cycle is the number of transport routes it contains.

Tight cycles are logistical nightmares. Find the length of the shortest dependency cycle.

Given the layout of the supply chain, determine the length of the shortest cycle.

## Examples

### 1

#### Input
5 6
1 2
1 3
2 4
2 5
3 4
4 5

#### Output
3

#### Explanation
There are several cycles in this network:
1-2-4-3-1 (length 4)
2-4-5-2 (length 3)
1-2-5-4-3-1 (length 5)
The shortest cycle has a length of 3.

### 2

#### Input
4 3
1 2
2 3
3 4

#### Output
-1

#### Explanation
The connections form a straight line (1-2-3-4). There are no cycles in this network.

## Input Format
- The first line contains two integers n and m: the number of factories and the number of transport routes.
- The factories are numbered 1, 2, ..., n.
- The next m lines describe the transport routes. Each line contains two integers u and v, indicating a connection between factory u and factory v.
- The graph is undirected. There is at most one transport route between any two factories.

## Output Format
- Return one integer: the length of the shortest cycle. If there are no cycles, print `-1`.

## Constraints
- 1 ≤ n ≤ 2500
- 1 ≤ m ≤ 5000
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph, breadth-first-search
