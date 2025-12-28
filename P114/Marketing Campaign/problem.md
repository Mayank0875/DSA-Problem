## Title
Marketing Campaign

## Slug
marketing-campaign

## Difficulty
Medium

## Description
Ads run in phases. A successful phase generates buzz to carry the campaign through future lull periods.

You start at the **first phase** (index 0). Each phase has a specific buzz factor, given by an integer array `nums`. The value at `nums[i]` represents the **maximum length** you can sustain forward from that position.

For example, if you are at index `i` and `nums[i] = 3`, you can sustain to any phase at index `i+1`, `i+2`, or `i+3`.

Your goal is to determine if it is possible to reach the **last phase** (the final index of the array) starting from the first.

Return `true` if you can reach the last index, or `false` otherwise.

## Examples

### 1

#### Input
5
2 3 1 1 4

#### Output
true

#### Explanation
Sustain 1 step from index 0 to 1, then sustain 3 steps to the last index.

### 2

#### Input
5
3 2 1 0 4

#### Output
false

#### Explanation
You will always arrive at index 3 no matter what. Its maximum sustain length is 0, which makes it impossible to advance further to the last index.

## Input Format
- The first line contains an integer `n`, the number of phases.
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
