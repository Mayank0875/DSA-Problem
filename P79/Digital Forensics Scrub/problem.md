## Title
Digital Forensics Scrub

## Slug
digital-forensics-scrub

## Difficulty
Medium

## Description
Hackers exfiltrate data. They scrub the connection logs, destroying the link after use.

The darknet consists of $n$ nodes and $m$ one-way tunnels. Each tunnel connects a specific source node to a destination node.

The process happens over several files. In each file, you must send a file from node 1 (the source) to node $n$ (the destination). The catch is that each tunnel is securely wiped and deleted after transfer. This means each tunnel can be used at most once across all files combined.

Your goal is to determine the maximum number of files you can successfully complete the journey from node 1 to node $n$.

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
You can complete 2 files.
Path 1: 1 -> 2 -> 6
Path 2: 1 -> 3 -> 4 -> 6 (or 1 -> 3 -> 5 -> 6)

### 2

#### Input
2 1
1 2

#### Output
1

#### Explanation
You can complete 1 file.

## Input Format
- The first line contains two integers $n$ and $m$: the number of nodes and the number of tunnels.
- The next $m$ lines describe the tunnels. Each line contains two integers $a$ and $b$, indicating a directed tunnel from node $a$ to node $b$.

## Output Format
- Return one integer: the maximum number of files possible.

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
