## Title

Strongest Signal Burst

## Slug

strongest-signal-burst

## Difficulty

Easy

## Description

A deep space probe sends back `n` data points, represented in a `Signal Array`. A "burst" is a contiguous sequence of `k` data points. Find the `maximum total strength (sum) from any contiguous 'k' data points` in the array.

Return the maximum sum that can be obtained.

## Examples

### 1

#### Input

5
1 2 3 4 5
2

#### Output

9

#### Explanation

All contiguous subarrays of size 2: `[1,2]=3`, `[2,3]=5`, `[3,4]=7`, `[4,5]=9`.  
Maximum sum is `9`.

### 2

#### Input

6
4 1 2 10 2 3
3

#### Output

15

#### Explanation

Subarrays of size 3: `[4,1,2]=7`, `[1,2,10]=13`, `[2,10,2]=14`, `[10,2,3]=15`.  
Maximum sum is `15`.

## Input Format  

- First line: integer `n` — size of the Cipher Sequence.  
- Second line: `n` space-separated integers — elements of the Cipher Sequence.  
- Third line: integer `k` — size of subarray.

## Output Format  

Return a single integer — maximum sum of any contiguous subarray of size `k`.



## Constraints  

- 1 ≤ n ≤ 1e4  
- -1e9 ≤ nums[i] ≤ 1e9  
- 0 ≤ k ≤ 1e4  

## Time Limit

1 second

## Memory Limit

512 MB

## Tags

arrays, sliding-window