## Title

Hiker's Maximum Energy Gain

## Slug

hikers-maximum-energy-gain

## Difficulty

Easy

## Description

A hiker is trekking across a mountain range. The range is represented by an array of integers, where each integer is the "energy value" of a specific checkpoint. The hiker wants to find the most energy they can collect during a single, continuous climb. A "continuous climb" is defined as a contiguous subarray of checkpoints where the energy value of each checkpoint is `strictly greater` than the previous one.

Your task is to find the maximum total energy the hiker can gain from one continuous climb. The climb must include at least one checkpoint.

## Examples

### 1

#### Input

6
[10, 20, 30, 5, 10, 50]

#### Output

65

#### Explanation

The hiker could climb `[10, 20, 30]` for a sum of 60. However, a better climb starts later: `[5, 10, 50]`. This is a strictly increasing contiguous subarray, and its sum is 65.
    
### 2

#### Input

5
[10, 20, 30, 40, 50]

#### Output

150

#### Explanation

The entire trail is a continuous climb. The sum of all checkpoints is 150.
  

## Input Format  

- The first line contains a single integer, `n`, the number of checkpoints.
- The second line contains `n` space-separated integers, representing the energy values `nums[i]` of the checkpoints.

## Output Format  

- Return a single integer representing the maximum sum of any strictly increasing contiguous subarray.
  

## Constraints  

- 1 ≤ n ≤ 100
- 1 ≤ nums[i] ≤ 100

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

array, sliding-window, easy