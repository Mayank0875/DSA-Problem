## Title
Bird Migration Altitude

## Slug
bird-migration-altitude

## Difficulty
Easy

## Description
A bird flock changes altitude n times. They try to find updrafts that take them strictly higher.

You have altitude logs for n points.
An ascent path consists of points where altitude is strictly higher than the previous point.

You must track the flight to find the longest possible ascent path. You can skip any number of points to form the sequence, but you must maintain the original flight path order of the selected points. Calculate the maximum number of points that can form such a sequence.

## Examples

### 1

#### Input
8
7 3 5 3 6 2 9 8

#### Output
4

#### Explanation
The input contains: [7, 3, 5, 3, 6, 2, 9, 8]. The longest ascent paths (strictly increasing) include:
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
Since the values are strictly decreasing, we can pick at most 1 point.

## Input Format
- The first line contains an integer n: the number of points.
- The second line contains n integers x_1, x_2 ... x_n: the altitude of each point in order.

## Output Format
- Return one integer: the length of the longest valid ascent path.

## Constraints
- 1 ≤ n ≤ 2e5
- 1 ≤ x ≤ 1e9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
binary-search, dynamic-programming, greedy
