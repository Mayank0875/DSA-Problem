## Title
Customer Service

## Slug
customer-service

## Difficulty
Medium

## Description
A support agent gets ratings. 1 is Positive, 0 is Negative. Management can expunge k negative reviews.

You review feedback ratings represented by an array `nums` consisting of 1s (positive reviews) and 0s (negative reviews), and an integer `k`. You are allowed to expunge at most `k` negative reviewss from the sequence.

Your task is to find the length of the longest contiguous sequence of positive reviewss after performing the expungements. If the sequence contains no positive reviewss even after optimal expungements, return 0.

## Examples

### 1

#### Input
4
1 1 0 1
1

#### Output
3

#### Explanation
After expunging the element at position 2 (value 0), the sequence becomes `[1, 1, 1]`. The longest segment of positive reviewss has length 3.

### 2

#### Input
9
0 1 1 1 0 1 1 0 1
2

#### Output
6

#### Explanation
We can expunge the negative reviews at index 4 and the negative reviews at index 7. The resulting segments of positive reviewss merge to form a sequence of length 6.

## Input Format
- The first line contains an integer `n`, representing the size of the array.
- The second line contains `n` space-separated integers representing the array `nums` (1 for positive reviews, 0 for negative reviews).
- The third line contains an integer `k`.

## Output Format
- Return a single integer representing the maximum size of the subarray of positive reviewss.

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
