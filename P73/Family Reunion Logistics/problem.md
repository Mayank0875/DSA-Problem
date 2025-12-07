## Title
Family Reunion Logistics

## Slug
family-reunion-logistics

## Difficulty
Medium

## Description
A large family tree has n members. Organizers want to find the best common ancestor to host a reunion for any k relatives.

The Organizer defines the "Hosting Potential" of the structure rooted at a specific member `r` as follows:
Consider every possible set of `k` distinct members from the structure.
1. For each set, find the Lowest Common Ancestor (LCA) of the members in that set, calculated with respect to the root `r`.
2. Let `S_r` be the set of all unique members obtained as LCAs from these sets.
3. The Hosting Potential of the structure rooted at `r` is the size of `S_r` (denoted as `|S_r|`).

The total "Family Connectivity" is defined as the sum of the Hosting Potential values for all possible roots `r` from 1 to `n`:
Family Connectivity = sum over `r` from 1 to `n` of `|S_r|`

Your task is to calculate the Family Connectivity of the given family tree.

Notes:
1. A family tree is a connected graph without cycles.
2. The LCA of a set of nodes in a rooted family tree is the deepest node that is an ancestor of all nodes in the set.

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
The calculated Family Connectivity is 17.

### 2

#### Input
2 2
1 2

#### Output
2

#### Explanation
The calculated Family Connectivity is 2.

## Input Format
- The first line of each test case contains two integers `n` and `k` — the number of members and the size of the sets to consider.
- The following `n-1` lines describe the family tree. Each line contains two integers `u` and `v`, indicating a connection between members `u` and `v`.

## Output Format
- Return one integer: the Family Connectivity.

## Constraints
- 1 ≤ k ≤ n ≤ 2e5
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
depth-first-search, graph
