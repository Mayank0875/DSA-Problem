## Title
Polymer Chain Stability

## Slug
polymer-chain-stability

## Difficulty
Medium

## Description
A chemist synthesizes a long polymer chain. A stable section of the chain is one that is composed of at most `k` distinct monomer types.

The polymer chain is represented as a sequence of monomers, where each monomer has a specific chemical ID. You need to select a contiguous segment of the sequence.

However, there is a constraint: the segment is valid only if it contains **at most** `k` distinct chemical IDs.

Given the sequence of monomers and the constraint `k`, your task is to calculate the total number of valid contiguous segments (subarrays).

## Examples

### 1

#### Input
5 2
1 2 3 1 1

#### Output
10

#### Explanation
The valid segments with at most 2 distinct values are:
[1], [2], [3], [1], [1] (length 1)
[1, 2], [2, 3], [3, 1], [1, 1] (length 2)
[3, 1, 1] (length 3)
Total = 10.

### 2

#### Input
5 1
1 2 3 4 5

#### Output
5

#### Explanation
Only single-element segments are valid because every pair has 2 distinct values, which exceeds k=1.

## Input Format
- The first line contains two integers `n` and `k`: the length of the sequence and the maximum allowed distinct values.
- The second line contains `n` integers representing the chemical IDs of the monomers.

## Output Format
- Return one integer: the number of valid contiguous segments.

## Constraints
- 1 ≤ k ≤ n ≤ 2e5
- 1 ≤ value ≤ 2e5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
sliding-window, two-pointers, array
