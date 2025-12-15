## Title
Training Weights

## Slug
training-weights

## Difficulty
Easy

## Description
An athlete lifts weights in n sessions. They want to log their 'progressive overload' sessions.

You have the weight lifted in n sessions.
A progressive log consists of sessions where the weight lifted is strictly heavier than the previous session.

You must review the log to find the longest possible progression. You can skip any number of sessions to form the sequence, but you must maintain the original chronological order of the selected sessions. Calculate the maximum number of sessions that can form such a sequence.

## Examples

### 1

#### Input
8
7 3 5 3 6 2 9 8

#### Output
4

#### Explanation
The input contains: [7, 3, 5, 3, 6, 2, 9, 8]. The longest progressions (strictly increasing) include:
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
Since the values are strictly decreasing, we can pick at most 1 session.

## Input Format
- The first line contains an integer n: the number of sessions.
- The second line contains n integers x_1, x_2 ... x_n: the weight of each session in order.

## Output Format
- Return one integer: the length of the longest valid progression.

## Constraints
- 1 ≤ n ≤ 2e5
- 1 ≤ x ≤ 1e9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
binary-search, dynamic-programming, greedy
