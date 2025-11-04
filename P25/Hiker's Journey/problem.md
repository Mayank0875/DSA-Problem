## Title

Hiker's Journey

## Slug

hikers-journey

## Difficulty

Medium

## Description

A hiker is planning a `k`-day trip. The trail consists of `n` consecutive sections, with section `i` having a length of `x[i]`. The hiker must complete the sections in order. Each day, they can hike a contiguous block of one or more sections. The hiker wants to minimize their "fatigue", which is defined by the longest distance they walk on any single day. Find the minimum possible value for the maximum distance walked in a day.

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

- The first line contains two integers `n` and `k`: the number of trail sections and the number of days.
- The second line contains `n` integers `x[1], x[2] ... x[n]`, where `x[i]` is the length of the i-th section.

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