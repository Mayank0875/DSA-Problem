## Title
Military Chain of Command

## Slug
military-chain-of-command

## Difficulty
Medium

## Description
An army structure has n units. The General Staff is analyzing command bottlenecks for squads of size k.

The General defines the "Command Influence" of the structure rooted at a specific unit `r` as follows:
Consider every possible set of `k` distinct units from the structure.
1. For each set, find the Lowest Common Ancestor (LCA) of the units in that set, calculated with respect to the root `r`.
2. Let `S_r` be the set of all unique units obtained as LCAs from these sets.
3. The Command Influence of the structure rooted at `r` is the size of `S_r` (denoted as `|S_r|`).

The total "Strategic Integrity" is defined as the sum of the Command Influence values for all possible roots `r` from 1 to `n`:
Strategic Integrity = sum over `r` from 1 to `n` of `|S_r|`

Your task is to calculate the Strategic Integrity of the given command structure.

Notes:
1. A command structure is a connected graph without cycles.
2. The LCA of a set of nodes in a rooted command structure is the deepest node that is an ancestor of all nodes in the set.

## Examples

### 1

#### Input
6 3
1 2
1 3
2 4
2 5
3 6

#### Output
17

#### Explanation
The calculated Strategic Integrity is 17.

### 2

#### Input
2 2
1 2

#### Output
2

#### Explanation
The calculated Strategic Integrity is 2.

## Input Format
- The first line of each test case contains two integers `n` and `k` — the number of units and the size of the sets to consider.
- The following `n-1` lines describe the command structure. Each line contains two integers `u` and `v`, indicating a connection between units `u` and `v`.

## Output Format
- Return one integer: the Strategic Integrity.

## Constraints
- 1 ≤ k ≤ n ≤ 2e5
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
depth-first-search, graph
