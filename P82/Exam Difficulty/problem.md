## Title
Exam Difficulty

## Slug
exam-difficulty

## Difficulty
Easy

## Description
A teacher creates a test from n questions. They want to pick questions that get strictly harder.

You have difficulty ratings for n questions.
A valid test consists of questions where the difficulty is strictly higher than the previous question.

You must create the test to find the longest possible valid test. You can skip any number of questions to form the sequence, but you must maintain the original pool order order of the selected questions. Calculate the maximum number of questions that can form such a sequence.

## Examples

### 1

#### Input
8
7 3 5 3 6 2 9 8

#### Output
4

#### Explanation
The input contains: [7, 3, 5, 3, 6, 2, 9, 8]. The longest valid tests (strictly increasing) include:
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
Since the values are strictly decreasing, we can pick at most 1 question.

## Input Format
- The first line contains an integer n: the number of questions.
- The second line contains n integers x_1, x_2 ... x_n: the difficulty of each question in order.

## Output Format
- Return one integer: the length of the longest valid valid test.

## Constraints
- 1 ≤ n ≤ 2e5
- 1 ≤ x ≤ 1e9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
binary-search, dynamic-programming, greedy
