## Title
Diamond Hardness Test

## Slug
diamond-hardness-test

## Difficulty
Easy

## Description
A geologist tests n minerals. They want to order them by strictly increasing hardness.

You have hardness values for n minerals.
A hardness scale consists of minerals where hardness is strictly higher than the previous one.

You must sort samples to find the longest possible hardness scale. You can skip any number of minerals to form the sequence, but you must maintain the original collection order order of the selected minerals. Calculate the maximum number of minerals that can form such a sequence.

## Examples

### 1

#### Input
8
7 3 5 3 6 2 9 8

#### Output
4

#### Explanation
The input contains: [7, 3, 5, 3, 6, 2, 9, 8]. The longest hardness scales (strictly increasing) include:
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
Since the values are strictly decreasing, we can pick at most 1 mineral.

## Input Format
- The first line contains an integer n: the number of minerals.
- The second line contains n integers x_1, x_2 ... x_n: the hardness of each mineral in order.

## Output Format
- Return one integer: the length of the longest valid hardness scale.

## Constraints
- 1 ≤ n ≤ 2e5
- 1 ≤ x ≤ 1e9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
binary-search, dynamic-programming, greedy
