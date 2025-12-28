## Title
Train Car Weights

## Slug
train-car-weights

## Difficulty
Medium

## Description
A freight train is assembled with lighter cars in front and heavier in back for physics reasons. A switching error placed random cars in the middle.

A valid train consist must be safe, meaning the weights should appear in non-decreasing order.

However, a signal error has inserted a chunk of incorrect weights into the middle of the train consist, corrupting it. To fix this, you must remove a single contiguous sequence of weights (a subarray) so that the remaining weights form a sorted, non-decreasing sequence.

Your goal is to minimize the cars uncoupled. Determine the length of the **shortest contiguous subarray** that needs to be removed to restore the non-decreasing order of the remaining weights.

## Examples

### 1

#### Input
8
1 2 3 10 4 2 3 5

#### Output
3

#### Explanation
The shortest subarray to remove is `[10, 4, 2]` (indices 3, 4, 5). The remaining train consist is `[1, 2, 3, 3, 5]`, which is sorted. Removing `[3, 10, 4]` is also a valid solution of length 3.

### 2

#### Input
5
5 4 3 2 1

#### Output
4

#### Explanation
Since the train consist is strictly decreasing, we can only keep one weight. We must remove a subarray of length 4 (e.g., `[5, 4, 3, 2]` leaving `[1]`).

## Input Format
- The first line contains an integer `n`, the number of weights.
- The second line contains `n` space-separated integers representing the `weights` array.

## Output Format
- Return a single integer representing the length of the shortest subarray to remove.

## Constraints
- 1 ≤ n ≤ 10^5
- 0 ≤ weights[i] ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, two-pointers, binary-search
