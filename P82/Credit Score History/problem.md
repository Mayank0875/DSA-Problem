## Title
Credit Score History

## Slug
credit-score-history

## Difficulty
Easy

## Description
A bank reviews n monthly credit scores. They look for a streak of credit improvement.

You have n credit scores.
An improvement streak consists of months where the score is strictly higher than the previously selected month.

You must evaluate the history to find the longest possible improvement streak. You can skip any number of scores to form the sequence, but you must maintain the original chronological order of the selected scores. Calculate the maximum number of scores that can form such a sequence.

## Examples

### 1

#### Input
8
7 3 5 3 6 2 9 8

#### Output
4

#### Explanation
The input contains: [7, 3, 5, 3, 6, 2, 9, 8]. The longest improvement streaks (strictly increasing) include:
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
Since the values are strictly decreasing, we can pick at most 1 score.

## Input Format
- The first line contains an integer n: the number of scores.
- The second line contains n integers x_1, x_2 ... x_n: the value of each score in order.

## Output Format
- Return one integer: the length of the longest valid improvement streak.

## Constraints
- 1 ≤ n ≤ 2e5
- 1 ≤ x ≤ 1e9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
binary-search, dynamic-programming, greedy
