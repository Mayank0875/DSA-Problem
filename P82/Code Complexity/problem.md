## Title
Code Complexity

## Slug
code-complexity

## Difficulty
Easy

## Description
A linter analyzes n functions. It flags a chain of functions that get progressively more complex.

You have complexity scores for n functions.
A complexity chain consists of functions where the score is strictly higher than the previous function.

You must analyze code to find the longest possible complexity chain. You can skip any number of functions to form the sequence, but you must maintain the original file order order of the selected functions. Calculate the maximum number of functions that can form such a sequence.

## Examples

### 1

#### Input
8
7 3 5 3 6 2 9 8

#### Output
4

#### Explanation
The input contains: [7, 3, 5, 3, 6, 2, 9, 8]. The longest complexity chains (strictly increasing) include:
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
Since the values are strictly decreasing, we can pick at most 1 function.

## Input Format
- The first line contains an integer n: the number of functions.
- The second line contains n integers x_1, x_2 ... x_n: the score of each function in order.

## Output Format
- Return one integer: the length of the longest valid complexity chain.

## Constraints
- 1 ≤ n ≤ 2e5
- 1 ≤ x ≤ 1e9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
binary-search, dynamic-programming, greedy
