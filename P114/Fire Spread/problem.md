## Title
Fire Spread

## Slug
fire-spread

## Difficulty
Medium

## Description
Fire jumps between trees. Dry trees allow the fire to spark further down the forest line.

You start at the **first tree** (index 0). Each tree has a specific flammability, given by an integer array `nums`. The value at `nums[i]` represents the **maximum length** you can spread forward from that position.

For example, if you are at index `i` and `nums[i] = 3`, you can spread to any tree at index `i+1`, `i+2`, or `i+3`.

Your goal is to determine if it is possible to reach the **last tree** (the final index of the array) starting from the first.

Return `true` if you can reach the last index, or `false` otherwise.

## Examples

### 1

#### Input
5
2 3 1 1 4

#### Output
true

#### Explanation
Spread 1 step from index 0 to 1, then spread 3 steps to the last index.

### 2

#### Input
5
3 2 1 0 4

#### Output
false

#### Explanation
You will always arrive at index 3 no matter what. Its maximum spread length is 0, which makes it impossible to advance further to the last index.

## Input Format
- The first line contains an integer `n`, the number of trees.
- The second line contains `n` space-separated integers representing the `nums` array.

## Output Format
- Return `true` if the last index is reachable, `false` otherwise.

## Constraints
- 1 ≤ n ≤ 10^4
- 0 ≤ nums[i] ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, dynamic-programming, greedy
