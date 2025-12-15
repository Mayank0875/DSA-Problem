## Title
Speed Dating Matches

## Slug
speed-dating-matches

## Difficulty
Easy

## Description
A participant rates n dates. They want to recall a sequence of dates that got progressively better.

You have ratings for n dates.
A progressive sequence consists of dates where the rating is strictly higher than the previous date.

You must recall dates to find the longest possible betterment chain. You can skip any number of dates to form the sequence, but you must maintain the original chronological order of the selected dates. Calculate the maximum number of dates that can form such a sequence.

## Examples

### 1

#### Input
8
7 3 5 3 6 2 9 8

#### Output
4

#### Explanation
The input contains: [7, 3, 5, 3, 6, 2, 9, 8]. The longest betterment chains (strictly increasing) include:
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
Since the values are strictly decreasing, we can pick at most 1 date.

## Input Format
- The first line contains an integer n: the number of dates.
- The second line contains n integers x_1, x_2 ... x_n: the rating of each date in order.

## Output Format
- Return one integer: the length of the longest valid betterment chain.

## Constraints
- 1 ≤ n ≤ 2e5
- 1 ≤ x ≤ 1e9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
binary-search, dynamic-programming, greedy
