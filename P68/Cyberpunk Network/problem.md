## Title
Cyberpunk Network

## Slug
cyberpunk-network

## Difficulty
Hard

## Description
In the neon-lit city of Neo-Veridia, hackers control n servers. Some servers are connected by secret data lines. The hacker collective 'Phantom 47' wants to consolidate control. They believe true power lies in networks whose total server count is a 'Phantom Number'—consisting only of digits 4 and 7.

You can splice new data lines to merge server networks. Merging k networks costs k - 1 new lines.

Your task is to determine the minimum number of extra data lines the hacker needs to build to create at least one network whose size is a Phantom Number. If this goal cannot be achieved, return -1.

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
The optimal way is to connect server 4 with server 3. We can also connect 4 with 1 or 2. This creates a network of size 4 (a Phantom Number).

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
There is no way to connect the servers to form a network with a size equal to a Phantom Number.

## Input Format
- The first line contains two integers n and m: the number of servers and the number of existing data lines.
- The next m lines each contain two integers u and v, representing a data line between server u and server v. Note that u may be equal to v, and there may be multiple data lines connecting the same pair of servers.

## Output Format
- Return a single integer: the minimum number of data lines to build. If no solution exists, print -1.

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
