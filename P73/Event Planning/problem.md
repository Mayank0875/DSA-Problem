## Title
Event Planning

## Slug
event-planning

## Difficulty
Medium

## Description
A festival has n events. Planners find main stages hosting k sub-events.

The Planner defines the "Stage Importance" of the structure rooted at a specific event `r` as follows:
Consider every possible set of `k` distinct events from the structure.
1. For each set, find the Lowest Common Ancestor (LCA) of the events in that set, calculated with respect to the root `r`.
2. Let `S_r` be the set of all unique events obtained as LCAs from these sets.
3. The Stage Importance of the structure rooted at `r` is the size of `S_r` (denoted as `|S_r|`).

The total "Festival Structure" is defined as the sum of the Stage Importance values for all possible roots `r` from 1 to `n`:
Festival Structure = sum over `r` from 1 to `n` of `|S_r|`

Your task is to calculate the Festival Structure of the given schedule tree.

Notes:
1. A schedule tree is a connected graph without cycles.
2. The LCA of a set of nodes in a rooted schedule tree is the deepest node that is an ancestor of all nodes in the set.

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
The calculated Festival Structure is 17.

### 2

#### Input
2 2
1 2

#### Output
2

#### Explanation
The calculated Festival Structure is 2.

## Input Format
- The first line of each test case contains two integers `n` and `k` — the number of events and the size of the sets to consider.
- The following `n-1` lines describe the schedule tree. Each line contains two integers `u` and `v`, indicating a connection between events `u` and `v`.

## Output Format
- Return one integer: the Festival Structure.

## Constraints
- 1 ≤ k ≤ n ≤ 2e5
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
depth-first-search, graph
