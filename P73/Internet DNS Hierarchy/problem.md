## Title
Internet DNS Hierarchy

## Slug
internet-dns-hierarchy

## Difficulty
Medium

## Description
The DNS system has n domains. Admins check which domains serve as authorities for groups of k subdomains.

The Admin defines the "Authority Level" of the structure rooted at a specific domain `r` as follows:
Consider every possible set of `k` distinct domains from the structure.
1. For each set, find the Lowest Common Ancestor (LCA) of the domains in that set, calculated with respect to the root `r`.
2. Let `S_r` be the set of all unique domains obtained as LCAs from these sets.
3. The Authority Level of the structure rooted at `r` is the size of `S_r` (denoted as `|S_r|`).

The total "DNS Structure Index" is defined as the sum of the Authority Level values for all possible roots `r` from 1 to `n`:
DNS Structure Index = sum over `r` from 1 to `n` of `|S_r|`

Your task is to calculate the DNS Structure Index of the given domain tree.

Notes:
1. A domain tree is a connected graph without cycles.
2. The LCA of a set of nodes in a rooted domain tree is the deepest node that is an ancestor of all nodes in the set.

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
The calculated DNS Structure Index is 17.

### 2

#### Input
2 2
1 2

#### Output
2

#### Explanation
The calculated DNS Structure Index is 2.

## Input Format
- The first line of each test case contains two integers `n` and `k` — the number of domains and the size of the sets to consider.
- The following `n-1` lines describe the domain tree. Each line contains two integers `u` and `v`, indicating a connection between domains `u` and `v`.

## Output Format
- Return one integer: the DNS Structure Index.

## Constraints
- 1 ≤ k ≤ n ≤ 2e5
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
depth-first-search, graph
