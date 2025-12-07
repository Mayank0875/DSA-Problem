## Title
School Curriculum

## Slug
school-curriculum

## Difficulty
Medium

## Description
A curriculum has n topics. Educators identify core concepts that link k advanced topics.

The Educator defines the "Concept Core" of the structure rooted at a specific topic `r` as follows:
Consider every possible set of `k` distinct topics from the structure.
1. For each set, find the Lowest Common Ancestor (LCA) of the topics in that set, calculated with respect to the root `r`.
2. Let `S_r` be the set of all unique topics obtained as LCAs from these sets.
3. The Concept Core of the structure rooted at `r` is the size of `S_r` (denoted as `|S_r|`).

The total "Curriculum Cohesion" is defined as the sum of the Concept Core values for all possible roots `r` from 1 to `n`:
Curriculum Cohesion = sum over `r` from 1 to `n` of `|S_r|`

Your task is to calculate the Curriculum Cohesion of the given learning tree.

Notes:
1. A learning tree is a connected graph without cycles.
2. The LCA of a set of nodes in a rooted learning tree is the deepest node that is an ancestor of all nodes in the set.

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
The calculated Curriculum Cohesion is 17.

### 2

#### Input
2 2
1 2

#### Output
2

#### Explanation
The calculated Curriculum Cohesion is 2.

## Input Format
- The first line of each test case contains two integers `n` and `k` — the number of topics and the size of the sets to consider.
- The following `n-1` lines describe the learning tree. Each line contains two integers `u` and `v`, indicating a connection between topics `u` and `v`.

## Output Format
- Return one integer: the Curriculum Cohesion.

## Constraints
- 1 ≤ k ≤ n ≤ 2e5
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
depth-first-search, graph
