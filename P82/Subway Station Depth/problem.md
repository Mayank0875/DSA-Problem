## Title
Subway Station Depth

## Slug
subway-station-depth

## Difficulty
Easy

## Description
A tunnel boring machine logs depths at n intervals. It must go deeper at each key point.

You have depth readings for n intervals.
A valid bore path consists of points where the depth is strictly greater than the previous point.

You must program the machine to find the longest possible bore path. You can skip any number of readings to form the sequence, but you must maintain the original distance order of the selected readings. Calculate the maximum number of readings that can form such a sequence.

## Examples

### 1

#### Input
8
7 3 5 3 6 2 9 8

#### Output
4

#### Explanation
The input contains: [7, 3, 5, 3, 6, 2, 9, 8]. The longest bore paths (strictly increasing) include:
3, 5, 6, 9
3, 5, 6, 8
The length of these sequences is 4.

### 2

#### Input
5
5 4 3 2 1

#### Output
1

#### Explanation
Since the values are strictly decreasing, we can pick at most 1 reading.

## Input Format
- The first line contains an integer n: the number of readings.
- The second line contains n integers x_1, x_2 ... x_n: the depth of each reading in order.

## Output Format
- Return one integer: the length of the longest valid bore path.

## Constraints
- 1 ≤ n ≤ 2e5
- 1 ≤ x ≤ 1e9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
binary-search, dynamic-programming, greedy
