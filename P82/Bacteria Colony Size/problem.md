## Title
Bacteria Colony Size

## Slug
bacteria-colony-size

## Difficulty
Easy

## Description
A lab tracks n petri dishes. They want to find a sequence of dishes showing clear growth stages.

You have population counts for n dishes.
A growth stage sequence consists of dishes where the population is strictly larger than the previous dish.

You must select dishes to find the longest possible growth stages. You can skip any number of dishes to form the sequence, but you must maintain the original experiment order of the selected dishes. Calculate the maximum number of dishes that can form such a sequence.

## Examples

### 1

#### Input
8
7 3 5 3 6 2 9 8

#### Output
4

#### Explanation
The input contains: [7, 3, 5, 3, 6, 2, 9, 8]. The longest growth stagess (strictly increasing) include:
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
Since the values are strictly decreasing, we can pick at most 1 dish.

## Input Format
- The first line contains an integer n: the number of dishes.
- The second line contains n integers x_1, x_2 ... x_n: the population of each dish in order.

## Output Format
- Return one integer: the length of the longest valid growth stages.

## Constraints
- 1 ≤ n ≤ 2e5
- 1 ≤ x ≤ 1e9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
binary-search, dynamic-programming, greedy
