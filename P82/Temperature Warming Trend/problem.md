## Title
Temperature Warming Trend

## Slug
temperature-warming-trend

## Difficulty
Easy

## Description
A climate scientist analyzes n daily temperature readings. They want to demonstrate a warming trend by picking days where the temperature strictly increases.

You are given n temperature readings.
A warming trend consists of days where the temperature is strictly higher than the previously selected day.

You must select data points to find the longest possible warming trend. You can skip any number of readings to form the sequence, but you must maintain the original chronological order of the selected readings. Calculate the maximum number of readings that can form such a sequence.

## Examples

### 1

#### Input
8
7 3 5 3 6 2 9 8

#### Output
4

#### Explanation
The input contains: [7, 3, 5, 3, 6, 2, 9, 8]. The longest warming trends (strictly increasing) include:
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
- The second line contains n integers x_1, x_2 ... x_n: the temperature of each reading in order.

## Output Format
- Return one integer: the length of the longest valid warming trend.

## Constraints
- 1 ≤ n ≤ 2e5
- 1 ≤ x ≤ 1e9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
binary-search, dynamic-programming, greedy
