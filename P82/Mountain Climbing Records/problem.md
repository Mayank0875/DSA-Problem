## Title
Mountain Climbing Records

## Slug
mountain-climbing-records

## Difficulty
Easy

## Description
A climber wants to log a series of peaks they summited. To show progress, they only want to list peaks where each subsequent peak is strictly higher than the one before it.

You have a log of n peaks climbed in order.
A progress log consists of peaks where the altitude of each chosen peak is strictly higher than the previous one.

You must select entries to find the longest possible ascent log. You can skip any number of peaks to form the sequence, but you must maintain the original chronological order of the selected peaks. Calculate the maximum number of peaks that can form such a sequence.

## Examples

### 1

#### Input
8
7 3 5 3 6 2 9 8

#### Output
4

#### Explanation
The input contains: [7, 3, 5, 3, 6, 2, 9, 8]. The longest ascent logs (strictly increasing) include:
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
Since the values are strictly decreasing, we can pick at most 1 peak.

## Input Format
- The first line contains an integer n: the number of peaks.
- The second line contains n integers x_1, x_2 ... x_n: the altitude of each peak in order.

## Output Format
- Return one integer: the length of the longest valid ascent log.

## Constraints
- 1 ≤ n ≤ 2e5
- 1 ≤ x ≤ 1e9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
binary-search, dynamic-programming, greedy
