## Title
Hiking Trail Fatigue

## Slug
hiking-trail-fatigue

## Difficulty
Hard

## Description
A hiker plans to walk a trail consisting of `n` segments over `k` days. Each segment has a specific length. The hiker must complete contiguous segments each day. The 'fatigue' for a day is calculated as the square of the total distance walked that day.

You must partition the sequence of segments into exactly `k` non-empty contiguous days.
Each day corresponds to a day.
The "fatigue" for a day is calculated as the **square of the sum** of the lengths of the segments in that day.

Your goal is to minimize the total fatigue (the sum of the fatigue values of all `k` days).

## Examples

### 1

#### Input
8 3
2 3 1 2 2 3 4 1

#### Output
110

#### Explanation
We partition the segments into 3 days: `[2, 3, 1]`, `[2, 2, 3]`, and `[4, 1]`.
The sums are 6, 7, 5.
The total fatigue is $6^2 + 7^2 + 5^2 = 36 + 49 + 25 = 110$.

### 2

#### Input
5 1
1 2 3 4 5

#### Output
225

#### Explanation
Only 1 day is allowed, containing all segments. Sum = 15. fatigue = $15^2 = 225$.

## Input Format
- The first line contains two integers `n` and `k`: the number of segments and the required number of days.
- The second line contains `n` integers representing the lengths of each segment.

## Output Format
- Return one integer: the minimum total fatigue.

## Constraints
- 1 ≤ k ≤ n ≤ 3000
- 1 ≤ value ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, array
