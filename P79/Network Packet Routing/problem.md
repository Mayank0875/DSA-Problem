## Title
Network Packet Routing

## Slug
network-packet-routing

## Difficulty
Medium

## Description
A sensitive data file is split into packets. To avoid interception, no two packets can use the same link.

The network consists of $n$ servers and $m$ one-way cables. Each cable connects a specific source server to a destination server.

The process happens over several packets. In each packet, you must send a packet from server 1 (the source) to server $n$ (the destination). The catch is that each cable is burned out after transmitting a single packet. This means each cable can be used at most once across all packets combined.

Your goal is to determine the maximum number of packets you can successfully complete the journey from server 1 to server $n$.

## Examples

### 1

#### Input
6 7
1 2
1 3
2 6
3 4
3 5
4 6
5 6

#### Output
2

#### Explanation
You can complete 2 packets.
Path 1: 1 -> 2 -> 6
Path 2: 1 -> 3 -> 4 -> 6 (or 1 -> 3 -> 5 -> 6)

### 2

#### Input
2 1
1 2

#### Output
1

#### Explanation
You can complete 1 packet.

## Input Format
- The first line contains two integers $n$ and $m$: the number of servers and the number of cables.
- The next $m$ lines describe the cables. Each line contains two integers $a$ and $b$, indicating a directed cable from server $a$ to server $b$.

## Output Format
- Return one integer: the maximum number of packets possible.

## Constraints
- 1 ≤ n ≤ 500
- 1 ≤ m ≤ 1000
- 1 ≤ a, b ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph, breadth-first-search
