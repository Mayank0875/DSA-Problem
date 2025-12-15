## Title
Mining Tunnel Collapse

## Slug
mining-tunnel-collapse

## Difficulty
Medium

## Description
Dangerous gas leaked in Shaft 1 and is drifting toward the Miners' Refuge (node n).

The mine consists of $n$ caverns connected by $m$ two-way tunnels.
The gas is attempting to travel from Shaft 1 (node 1) to the Refuge (node $n$).

To prevent this, you can detonate specific tunnels. Detonating a tunnel seals it off.

Your task is to calculate the **minimum number of tunnels** that must be detonated to completely sever all routes between Shaft 1 and the Refuge.

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
We can detonate edges (1,3) and (2,3) to isolate node 3.

## Input Format
- The first line contains two integers $n$ and $m$: the number of caverns and tunnels.
- The next $m$ lines describe the tunnels. Each line contains two integers $a$ and $b$, indicating a tunnel between cavern $a$ and cavern $b$.

## Output Format
- Return one integer: the minimum number of tunnels that need to be detonated.

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
