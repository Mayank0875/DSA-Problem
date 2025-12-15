## Title
Archaeological Dig Layers

## Slug
archaeological-dig-layers

## Difficulty
Hard

## Description
A site has `n` soil layers. The team excavates in `k` phases. Layers must be removed top-down. The 'equipment wear' for a phase is the square of the total depth excavated.

You must partition the sequence of layers into exactly `k` non-empty contiguous phases.
Each phase corresponds to a phase.
The "equipment wear" for a phase is calculated as the **square of the sum** of the depths of the layers in that phase.

Your goal is to minimize the total equipment wear (the sum of the equipment wear values of all `k` phases).

## Examples

### 1

#### Input
8 3
2 3 1 2 2 3 4 1

#### Output
110

#### Explanation
We partition the layers into 3 phases: `[2, 3, 1]`, `[2, 2, 3]`, and `[4, 1]`.
The sums are 6, 7, 5.
The total equipment wear is $6^2 + 7^2 + 5^2 = 36 + 49 + 25 = 110$.

### 2

#### Input
5 1
1 2 3 4 5

#### Output
225

#### Explanation
Only 1 phase is allowed, containing all layers. Sum = 15. equipment wear = $15^2 = 225$.

## Input Format
- The first line contains two integers `n` and `k`: the number of layers and the required number of phases.
- The second line contains `n` integers representing the depths of each layer.

## Output Format
- Return one integer: the minimum total equipment wear.

## Constraints
- 1 ≤ k ≤ n ≤ 3000
- 1 ≤ value ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, array
