## Title
Electron Flow

## Slug
electron-flow

## Difficulty
Medium

## Description
A physicist creates a circuit. Electrons must flow to the Anode.

There are $n$ components numbered from $1$ to $n$, connected by $n-1$ wires. The network forms a tree structure (there is exactly one path between any two components). Currently, all wires are one-way.

Physics dictates charge movement to the **Anode (Node 1)**. To ensure success, every other component must be able to reach Anode by traveling along the wires in the correct direction.

You are given the current orientation of the wires. Your task is to determine the **minimum** number of wires that need to be polarized so that every component can reach Anode.

## Examples

### 1

#### Input
6
1 2
2 4
3 2
5 1
5 6

#### Output
3

#### Explanation
The destination is Anode (1).
- Wire 1->2 points away from 1. Needs polarization.
- Wire 2->4 points away from 1. Needs polarization.
- Wire 3->2 points towards 2 (and effectively towards 1). OK.
- Wire 5->1 points towards 1. OK.
- Wire 5->6 points away from 1 (via 5). Needs polarization.
Total polarizations: 3.

### 2

#### Input
5
2 1
2 3
4 3
4 5

#### Output
2

#### Explanation
Wires 2->3 and 4->5 need to be polarized.

## Input Format
- The first line contains an integer $n$ — the number of components.
- The next $n-1$ lines each contain two integers $u$ and $v$, representing a one-way wire from component $u$ to component $v$.

## Output Format
- Return a single integer representing the minimum number of wires that need to be changed.

## Constraints
- 1 ≤ n ≤ 10^5
- 1 ≤ u, v ≤ n
- The graph is guaranteed to be a tree.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
tree, depth-first-search, breadth-first-search, graph

## Company
google, amazon
