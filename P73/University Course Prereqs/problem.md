## Title
University Course Prereqs

## Slug
university-course-prereqs

## Difficulty
Medium

## Description
A college has n courses. The Dean finds foundational courses needed for k majors.

The Dean defines the "Foundational Value" of the structure rooted at a specific course `r` as follows:
Consider every possible set of `k` distinct courses from the structure.
1. For each set, find the Lowest Common Ancestor (LCA) of the courses in that set, calculated with respect to the root `r`.
2. Let `S_r` be the set of all unique courses obtained as LCAs from these sets.
3. The Foundational Value of the structure rooted at `r` is the size of `S_r` (denoted as `|S_r|`).

The total "Academic Core Score" is defined as the sum of the Foundational Value values for all possible roots `r` from 1 to `n`:
Academic Core Score = sum over `r` from 1 to `n` of `|S_r|`

Your task is to calculate the Academic Core Score of the given prerequisite tree.

Notes:
1. A prerequisite tree is a connected graph without cycles.
2. The LCA of a set of nodes in a rooted prerequisite tree is the deepest node that is an ancestor of all nodes in the set.

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
The calculated Academic Core Score is 17.

### 2

#### Input
2 2
1 2

#### Output
2

#### Explanation
The calculated Academic Core Score is 2.

## Input Format
- The first line of each test case contains two integers `n` and `k` — the number of courses and the size of the sets to consider.
- The following `n-1` lines describe the prerequisite tree. Each line contains two integers `u` and `v`, indicating a connection between courses `u` and `v`.

## Output Format
- Return one integer: the Academic Core Score.

## Constraints
- 1 ≤ k ≤ n ≤ 2e5
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
depth-first-search, graph
