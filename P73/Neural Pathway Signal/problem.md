## Title
Neural Pathway Signal

## Slug
neural-pathway-signal

## Difficulty
Medium

## Description
A brain scan maps n neurons. Neuroscientists study how signals from k neurons converge at processing nodes.

The Scientist defines the "Signal Convergence" of the structure rooted at a specific neuron `r` as follows:
Consider every possible set of `k` distinct neurons from the structure.
1. For each set, find the Lowest Common Ancestor (LCA) of the neurons in that set, calculated with respect to the root `r`.
2. Let `S_r` be the set of all unique neurons obtained as LCAs from these sets.
3. The Signal Convergence of the structure rooted at `r` is the size of `S_r` (denoted as `|S_r|`).

The total "Neural Complexity" is defined as the sum of the Signal Convergence values for all possible roots `r` from 1 to `n`:
Neural Complexity = sum over `r` from 1 to `n` of `|S_r|`

Your task is to calculate the Neural Complexity of the given neural pathway.

Notes:
1. A neural pathway is a connected graph without cycles.
2. The LCA of a set of nodes in a rooted neural pathway is the deepest node that is an ancestor of all nodes in the set.

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
The calculated Neural Complexity is 17.

### 2

#### Input
2 2
1 2

#### Output
2

#### Explanation
The calculated Neural Complexity is 2.

## Input Format
- The first line of each test case contains two integers `n` and `k` — the number of neurons and the size of the sets to consider.
- The following `n-1` lines describe the neural pathway. Each line contains two integers `u` and `v`, indicating a connection between neurons `u` and `v`.

## Output Format
- Return one integer: the Neural Complexity.

## Constraints
- 1 ≤ k ≤ n ≤ 2e5
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
depth-first-search, graph
