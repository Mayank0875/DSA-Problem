## Title
Code Linting

## Slug
code-linting

## Difficulty
Medium

## Description
A linter checks lines of code. 1 is Compliant, 0 is Violation. An auto-fixer can correct k violations.

You run a code linter represented by an array `nums` consisting of 1s (compliant lines) and 0s (violations), and an integer `k`. You are allowed to fix at most `k` violationss from the sequence.

Your task is to find the length of the longest contiguous sequence of compliant liness after performing the fixes. If the sequence contains no compliant liness even after optimal fixes, return 0.

## Examples

### 1

#### Input
4
1 1 0 1
1

#### Output
3

#### Explanation
After fixing the element at position 2 (value 0), the sequence becomes `[1, 1, 1]`. The longest segment of compliant liness has length 3.

### 2

#### Input
9
0 1 1 1 0 1 1 0 1
2

#### Output
6

#### Explanation
We can fix the violations at index 4 and the violations at index 7. The resulting segments of compliant liness merge to form a sequence of length 6.

## Input Format
- The first line contains an integer `n`, representing the size of the array.
- The second line contains `n` space-separated integers representing the array `nums` (1 for compliant lines, 0 for violations).
- The third line contains an integer `k`.

## Output Format
- Return a single integer representing the maximum size of the subarray of compliant liness.

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
