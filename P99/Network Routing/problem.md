## Title
Network Routing

## Slug
network-routing

## Difficulty
Hard

## Description
Admins route packets through servers. Servers forward to specific next hops.

Admin and Hacker are playing a strategic game using a routing table $p$ of length $n$. The game starts with a bandwidth of 0.

The players take turns, with Admin moving first. On each turn, a player chooses an integer $x$ from the routing table that has not been chosen before.
- If it is Admin's turn, the chosen value $x$ is **added** to the bandwidth.
- If it is Hacker's turn, the chosen value $x$ is **subtracted** from the bandwidth.

The rules for choosing $x$ are:
1. On the very first move of the game, Admin may choose **any** unselected server from the routing table.
2. On every move after the first:
   - Let $m$ be the index of the server chosen in the previous move (that is, the previous player chose $p[m]$).
   - If the value $p[m]$ has not yet been chosen, the current player **must** choose $p[m]$.
   - If $p[m]$ has already been chosen, the current player may choose **any** unselected server.

The game continues until all servers of the routing table have been chosen.

Admin plays optimally to **maximize** the final bandwidth, while Hacker plays optimally to **minimize** it.

Your task is to compute the final bandwidth assuming both players play optimally.

## Examples

### 1

#### Input
3
2 3 1

#### Output
4

#### Explanation
Final bandwidth is 4.

### 2

#### Input
2
2 1

#### Output
1

#### Explanation
Final bandwidth is 1.

## Input Format
- The first line contains an integer $n$ (length of routing table).
- The second line contains $n$ space-separated integers $p_1, \dots, p_n$.

## Output Format
- Return one integer: the final bandwidth on a new line.

## Constraints
- 1 ≤ n ≤ 10^6
- 1 ≤ p_i ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
greedy, graph, combinatorics
