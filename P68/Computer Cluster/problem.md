## Title
Computer Cluster

## Slug
computer-cluster

## Difficulty
Hard

## Description
A supercomputer has n processing nodes. Cables link them into clusters. Processing efficiency peaks if a cluster has a 'Binary-Like' size (digits 4 and 7).

An admin can add cables. Merging k clusters costs k - 1 cables.

Your task is to determine the minimum number of extra cables the admin needs to build to create at least one cluster whose size is a Binary-Like Number. If this goal cannot be achieved, return -1.

## Examples

### 1

#### Input
4 3
1 2
2 3
1 3

#### Output
1

#### Explanation
The optimal way is to connect node 4 with node 3. We can also connect 4 with 1 or 2. This creates a cluster of size 4 (a Binary-Like Number).

### 2

#### Input
5 4
1 2
3 4
4 5
3 5

#### Output
-1

#### Explanation
There is no way to connect the nodes to form a cluster with a size equal to a Binary-Like Number.

## Input Format
- The first line contains two integers n and m: the number of nodes and the number of existing cables.
- The next m lines each contain two integers u and v, representing a cable between node u and node v. Note that u may be equal to v, and there may be multiple cables connecting the same pair of nodes.

## Output Format
- Return a single integer: the minimum number of cables to build. If no solution exists, print -1.

## Constraints
- 1 ≤ n ≤ 1e5
- 1 ≤ m ≤ 2e5
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph, dynamic-programming

## Companies
infosys
