## Title
Growth Spurt Analysis

## Slug
growth-spurt-analysis

## Difficulty
Easy

## Description
A biologist tracks the height of a plant daily. They want to identify the longest period of strictly continuous growth spurts from the data.

You have n daily height measurements.
A growth spurt sequence consists of days where the height measurement is strictly greater than the previous selected day's measurement.

You must analyze the data to find the longest possible growth sequence. You can skip any number of measurements to form the sequence, but you must maintain the original chronological order of the selected measurements. Calculate the maximum number of measurements that can form such a sequence.

## Examples

### 1

#### Input
8
7 3 5 3 6 2 9 8

#### Output
4

#### Explanation
The input contains: [7, 3, 5, 3, 6, 2, 9, 8]. The longest growth sequences (strictly increasing) include:
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
Since the values are strictly decreasing, we can pick at most 1 measurement.

## Input Format
- The first line contains an integer n: the number of measurements.
- The second line contains n integers x_1, x_2 ... x_n: the height of each measurement in order.

## Output Format
- Return one integer: the length of the longest valid growth sequence.

## Constraints
- 1 ≤ n ≤ 2e5
- 1 ≤ x ≤ 1e9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
binary-search, dynamic-programming, greedy
