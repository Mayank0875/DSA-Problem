## Title

Secure Network Message Routing

## Slug

secure-network-message-routing

## Difficulty

Medium

## Description

Alice needs to send a classified packet from source server 1 to destination server n. The network has n servers and m directed links. Links may repeat between the same pair of servers and self-loops are allowed. A path of length k is a sequence of exactly k directed links; nodes and links may be visited multiple times.

Given n, m, k and a list of the m directed links (each link given as two integers u v meaning a directed edge from u to v), compute the number of distinct paths that start at server 1 and end at server n with length exactly k. Output the answer modulo 1000000007.

## Examples

### 1

#### Input

3 4 8
1 2
2 3
3 1
3 2

#### Output

2

#### Explanation

Graph: 3 nodes. We want the number of directed paths of length 8 from node 1 to node 3. This is the (1,3) entry of M^8, where M is the adjacency matrix.

The valid length-8 paths from 1 to 3 you listed are:
1 → 2 → 3 → 1 → 2 → 3 → 1 → 2 → 3
1 → 2 → 3 → 2 → 3 → 1 → 2 → 3
So there are 2 such paths. Therefore the (1,3) entry of M^8 equals 2 (using 1-based node indexing).
    
### 2

#### Input

3 4 2
1 2
2 3
3 1
3 2

#### Output

1

#### Explanation

Yes — assuming the graph has edges 1→2 and 2→3 and there is no direct edge 1→3 (and no other way through node 1,2,3), the only path of length 2 from node 1 to node 3 is:
1 → 2 → 3
  

## Input Format  

- The first line contains three integers n, m, and k: the number of nodes, edges, and the required path length.
- The next m lines describe the edges. Each line contains two integers a and b, indicating a directed edge from node a to node b.

## Output Format  

- Return single integer: the number of paths modulo $10^9+7$.
  

## Constraints  

- 1 ≤ n ≤ 100
- 1 ≤ m ≤ 1e5
- 1 ≤ k ≤ 1e18
- 1 ≤ a, b ≤ n


## Time Limit

2 second

## Memory Limit

256 MB

## Tags

graph, dynamic-programming, hackwithinfy

## Companies
infosys