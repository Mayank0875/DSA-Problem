## Title

Road Trip Planning

## Slug

road-trip-planning

## Difficulty

Medium

## Description

You are planning a road trip across `n` consecutive highway segments. Each segment `i` has a length of `x[i]` miles. You are planning the trip for `k` days. You must travel the segments in order, and each day you must complete a contiguous block of segments (e.g., Day 1: segments 1-3, Day 2: segments 4-5, etc.). You want to make the trip relaxing, so you aim to minimize the longest distance driven on any single day. Find the minimum possible value for the maximum distance driven in one day.

## Examples

### 1

#### Input

5 3 
2 4 7 3 5


#### Output

8

#### Explanation

An optimal distribution assigns scrolls [2, 4] to the first scribe (sum 6 pages), scroll [7] to the second scribe (sum 7 pages), and scrolls [3, 5] to the third scribe (sum 8 pages). The maximum number of pages assigned to any scribe is 8. No other distribution into 3 contiguous blocks can achieve a maximum load less than 8.

### 2

#### Input

1 1
34

#### Output

34


#### Explanation

No other distribution into 1 contiguous blocks can achieve a maximum load less than 34.

## Input Format

- The first line contains two integers `n` and `k`: the number of highway segments and the number of days.
- The second line contains `n` integers `x[1], x[2] ... x[n]`, where `x[i]` is the length of the i-th segment.

## Output Format

- Return one integer: the minimum possible value for the maximum number of pages assigned to any scribe.

## Constraints

- 1 ≤ k ≤ n ≤ 2e5
- 1 ≤ x[i] ≤ 10^9

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

binary-search, greedy