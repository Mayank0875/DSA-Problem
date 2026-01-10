## Title
Code Compilation

## Slug
code-compilation

## Difficulty
Medium

## Description
A script runs daily. 1 is Success, 0 is Error. A debugger script can auto-resolve k errors.

You check build logs represented by an array `nums` consisting of 1s (successful builds) and 0s (errors), and an integer `k`. You are allowed to resolve at most `k` errorss from the sequence.

Your task is to find the length of the longest contiguous sequence of successful buildss after performing the resolutions. If the sequence contains no successful buildss even after optimal resolutions, return 0.

## Examples

### 1

#### Input
4
1 1 0 1
1

#### Output
3

#### Explanation
After resolving the element at position 2 (value 0), the sequence becomes `[1, 1, 1]`. The longest segment of successful buildss has length 3.

### 2

#### Input
9
0 1 1 1 0 1 1 0 1
2

#### Output
6

#### Explanation
We can resolve the errors at index 4 and the errors at index 7. The resulting segments of successful buildss merge to form a sequence of length 6.

## Input Format
- The first line contains an integer `n`, representing the size of the array.
- The second line contains `n` space-separated integers representing the array `nums` (1 for successful builds, 0 for errors).
- The third line contains an integer `k`.

## Output Format
- Return a single integer representing the maximum size of the subarray of successful buildss.

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
