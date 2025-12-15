## Title
Network Security Breach

## Slug
network-security-breach

## Difficulty
Medium

## Description
A hacker has compromised the Entry Server (node 1) and is trying to reach the Core Database (node n).

The network consists of $n$ servers connected by $m$ two-way data cables.
The malware is attempting to travel from the Entry Server (node 1) to the Core DB (node $n$).

To prevent this, you can cut specific data cables. Cutting a cable stops data transfer.

Your task is to calculate the **minimum number of data cables** that must be cut to completely sever all routes between the Entry Server and the Core DB.

## Examples

### 1

#### Input
4 5
1 2
1 3
2 3
3 4
1 4

#### Output
2

#### Explanation
The minimum is 2.

### 2

#### Input
3 3
1 2
2 3
1 3

#### Output
2

#### Explanation
We can cut edges (1,3) and (2,3) to isolate node 3.

## Input Format
- The first line contains two integers $n$ and $m$: the number of servers and data cables.
- The next $m$ lines describe the data cables. Each line contains two integers $a$ and $b$, indicating a data cable between server $a$ and server $b$.

## Output Format
- Return one integer: the minimum number of data cables that need to be cut.

## Constraints
- 1 ≤ n ≤ 500
- 1 ≤ m ≤ 1000
- 1 ≤ a, b ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph
