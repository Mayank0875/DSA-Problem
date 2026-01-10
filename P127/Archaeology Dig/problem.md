## Title
Archaeology Dig

## Slug
archaeology-dig

## Difficulty
Medium

## Description
A team sifts soil layers. 1 is Artifact, 0 is Dirt. They can discard k layers of dirt to find continuous artifacts.

You sift through layers represented by an array `nums` consisting of 1s (artifact layers) and 0s (dirt layers), and an integer `k`. You are allowed to discard at most `k` dirt layerss from the sequence.

Your task is to find the length of the longest contiguous sequence of artifact layerss after performing the discards. If the sequence contains no artifact layerss even after optimal discards, return 0.

## Examples

### 1

#### Input
4
1 1 0 1
1

#### Output
3

#### Explanation
After discarding the element at position 2 (value 0), the sequence becomes `[1, 1, 1]`. The longest segment of artifact layerss has length 3.

### 2

#### Input
9
0 1 1 1 0 1 1 0 1
2

#### Output
6

#### Explanation
We can discard the dirt layers at index 4 and the dirt layers at index 7. The resulting segments of artifact layerss merge to form a sequence of length 6.

## Input Format
- The first line contains an integer `n`, representing the size of the array.
- The second line contains `n` space-separated integers representing the array `nums` (1 for artifact layers, 0 for dirt layers).
- The third line contains an integer `k`.

## Output Format
- Return a single integer representing the maximum size of the subarray of artifact layerss.

## Constraints
- 1 ≤ n ≤ 10^5
- 0 ≤ nums[i] ≤ 1
- 0 ≤ k ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
sliding-window, two-pointers, array

## Company
facebook
