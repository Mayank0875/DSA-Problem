## Title
Internet Routing

## Slug
internet-routing

## Difficulty
Medium

## Description
BGP routers announce paths. A routing loop causes packets to circle until TTL expires.

A "routing loop" occurs when a packet moves from a router, through a sequence of links, and returns to the starting router without traversing the same link twice in immediate succession. The "length" of such a routing loop is the number of links it contains.

Tight loops congest the core. Find the hop count of the shortest routing loop.

Given the layout of the internet, determine the length of the shortest routing loop.

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
There are several routing loops in this network:
1-2-4-3-1 (length 4)
2-4-5-2 (length 3)
1-2-5-4-3-1 (length 5)
The shortest routing loop has a length of 3.

### 2

#### Input
4 3
1 2
2 3
3 4

#### Output
-1

#### Explanation
The connections form a straight line (1-2-3-4). There are no routing loops in this network.

## Input Format
- The first line contains two integers n and m: the number of routers and the number of links.
- The routers are numbered 1, 2, ..., n.
- The next m lines describe the links. Each line contains two integers u and v, indicating a connection between router u and router v.
- The graph is undirected. There is at most one link between any two routers.

## Output Format
- Return one integer: the length of the shortest routing loop. If there are no routing loops, print `-1`.

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
