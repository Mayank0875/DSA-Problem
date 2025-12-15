## Title
Coral Reef Spawning

## Slug
coral-reef-spawning

## Difficulty
Medium

## Description
Gametes float on currents. Currents shift unpredictably after carrying a batch.

The reef consists of $n$ corals and $m$ one-way currents. Each current connects a specific source coral to a destination coral.

The process happens over several spawns. In each spawn, you must send a spawn cloud from coral 1 (the source) to coral $n$ (the destination). The catch is that each current shifts direction and becomes unusable. This means each current can be used at most once across all spawns combined.

Your goal is to determine the maximum number of spawns you can successfully complete the journey from coral 1 to coral $n$.

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
You can complete 2 spawns.
Path 1: 1 -> 2 -> 6
Path 2: 1 -> 3 -> 4 -> 6 (or 1 -> 3 -> 5 -> 6)

### 2

#### Input
2 1
1 2

#### Output
1

#### Explanation
You can complete 1 spawn.

## Input Format
- The first line contains two integers $n$ and $m$: the number of corals and the number of currents.
- The next $m$ lines describe the currents. Each line contains two integers $a$ and $b$, indicating a directed current from coral $a$ to coral $b$.

## Output Format
- Return one integer: the maximum number of spawns possible.

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
