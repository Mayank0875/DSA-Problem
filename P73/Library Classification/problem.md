## Title
Library Classification

## Slug
library-classification

## Difficulty
Medium

## Description
A library system classifies n subjects. Librarians find the general categories covering sets of k specific topics.

The Librarian defines the "Category Breadth" of the structure rooted at a specific subject `r` as follows:
Consider every possible set of `k` distinct subjects from the structure.
1. For each set, find the Lowest Common Ancestor (LCA) of the subjects in that set, calculated with respect to the root `r`.
2. Let `S_r` be the set of all unique subjects obtained as LCAs from these sets.
3. The Category Breadth of the structure rooted at `r` is the size of `S_r` (denoted as `|S_r|`).

The total "Classification Depth" is defined as the sum of the Category Breadth values for all possible roots `r` from 1 to `n`:
Classification Depth = sum over `r` from 1 to `n` of `|S_r|`

Your task is to calculate the Classification Depth of the given subject tree.

Notes:
1. A subject tree is a connected graph without cycles.
2. The LCA of a set of nodes in a rooted subject tree is the deepest node that is an ancestor of all nodes in the set.

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
The calculated Classification Depth is 17.

### 2

#### Input
2 2
1 2

#### Output
2

#### Explanation
The calculated Classification Depth is 2.

## Input Format
- The first line of each test case contains two integers `n` and `k` — the number of subjects and the size of the sets to consider.
- The following `n-1` lines describe the subject tree. Each line contains two integers `u` and `v`, indicating a connection between subjects `u` and `v`.

## Output Format
- Return one integer: the Classification Depth.

## Constraints
- 1 ≤ k ≤ n ≤ 2e5
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
depth-first-search, graph
