## Title
Fungal Mycelium Growth

## Slug
fungal-mycelium-growth

## Difficulty
Medium

## Description
Fungal nodes exchange nutrients. Adjacent nodes pair up to form fruiting bodies. Each node contributes to one body.

The structure is a tree with n nodes and n-1 hyphae.
A fruiting body is formed between two nodes connected by a hypha.
However, each node can be part of at most one fruiting body.

Your task is to calculate the maximum number of fruiting bodys that can be formed.

## Examples

### 1

#### Input
5
1 2
1 3
3 4
3 5

#### Output
2

#### Explanation
One optimal set of fruiting bodys is (1, 2) and (3, 4). Node 5 remains unpaired. This gives a total of 2 fruiting bodys.

### 2

#### Input
4
1 2
2 3
3 4

#### Output
2

#### Explanation
We can form fruiting bodys (1, 2) and (3, 4), giving a total of 2.

## Input Format
- The first line contains an integer n, the number of nodes.
- The next n-1 lines each contain two integers u and v, representing a hypha between node u and node v.

## Output Format
- Return a single integer representing the maximum number of fruiting bodys.

## Constraints
- 1 ≤ n ≤ 2e5
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, graph
