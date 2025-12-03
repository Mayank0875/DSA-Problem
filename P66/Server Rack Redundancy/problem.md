## Title
Server Rack Redundancy

## Slug
server-rack-redundancy

## Difficulty
Medium

## Description
A data center needs a redundant cable layout between two rows of servers.

Two parallel racks, Row A and Row B, each contain n servers arranged in a line.
Row A has an array `a` representing the processing load of each server.
Row B has an array `b` representing the processing load of each server.

Inside each rack, adjacent servers are already connected by internal local bus lines.

You must establish inter-rack cross-connect cables connecting some servers of Row A to some servers of Row B.

The cost to create a cable between server i of Row A and server j of Row B is:
absolute value of (a[i] - b[j]).

**Fault-tolerance requirement:**
The final network must remain fully connected even if any single server is removed (from either Row A or Row B).
If one server fails and disappears along with all its connections, the remaining servers must still form a single connected network.

Your task is to calculate the minimum total cost required to build such a set of connections.

## Examples

### 1

#### Input
3
1 10 1
20 4 25

#### Output
31

#### Explanation
It's optimal to connect four pairs of servers:
1. server 1 from Row A with server 2 from Row B: cost |1-4| = 3.
2. server 3 from Row A with server 2 from Row B: cost |1-4| = 3.
3. server 2 from Row A with server 1 from Row B: cost |10-20| = 10.
4. server 2 from Row A with server 3 from Row B: cost |10-25| = 15.
Total cost: 3 + 3 + 10 + 15 = 31.

### 2

#### Input
4
1 1 1 1
1000000000 1000000000 1000000000 1000000000

#### Output
1999999998

#### Explanation
It is optimal to connect the first server of Row A with the first of Row B, and the last server of Row A with the last of Row B, satisfying the connectivity conditions efficiently given the values.

## Input Format
- The first line contains an integer n, the number of servers in each rack.
- The second line contains n integers representing the processing loads of Row A.
- The third line contains n integers representing the processing loads of Row B.

## Output Format
- Return a single integer representing the minimum total cost to make the network fault-tolerant.

## Constraints
- 3 ≤ n ≤ 10^5
- 1 ≤ a[i], b[i] ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph, greedy, math
