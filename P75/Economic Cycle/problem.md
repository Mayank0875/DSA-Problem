## Title
Economic Cycle

## Slug
economic-cycle

## Difficulty
Medium

## Description
Economists track money flow. A cycle occurs when money spent eventually returns to the spender through trade.

A "trade cycle" occurs when currency moves from a market, through a sequence of channels, and returns to the starting market without traversing the same transaction channel twice in immediate succession. The "length" of such a trade cycle is the number of channels it contains.

Fast cycles indicate high velocity of money. Find the length of the shortest trade loop.

Given the layout of the economy, determine the length of the shortest trade cycle.

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
There are several trade cycles in this network:
1-2-4-3-1 (length 4)
2-4-5-2 (length 3)
1-2-5-4-3-1 (length 5)
The shortest trade cycle has a length of 3.

### 2

#### Input
4 3
1 2
2 3
3 4

#### Output
-1

#### Explanation
The connections form a straight line (1-2-3-4). There are no trade cycles in this network.

## Input Format
- The first line contains two integers n and m: the number of markets and the number of channels.
- The markets are numbered 1, 2, ..., n.
- The next m lines describe the channels. Each line contains two integers u and v, indicating a connection between market u and market v.
- The graph is undirected. There is at most one transaction channel between any two markets.

## Output Format
- Return one integer: the length of the shortest trade cycle. If there are no trade cycles, print `-1`.

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
