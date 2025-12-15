## Title
Server Upgrades

## Slug
server-upgrades

## Difficulty
Easy

## Description
An IT manager reviews n server models. They want to implement an upgrade path of strictly increasing RAM.

You have RAM sizes for n models.
An upgrade path consists of models where RAM is strictly higher than the previous model.

You must plan upgrades to find the longest possible upgrade path. You can skip any number of models to form the sequence, but you must maintain the original catalog order order of the selected models. Calculate the maximum number of models that can form such a sequence.

## Examples

### 1

#### Input
8
7 3 5 3 6 2 9 8

#### Output
4

#### Explanation
The input contains: [7, 3, 5, 3, 6, 2, 9, 8]. The longest upgrade paths (strictly increasing) include:
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
Since the values are strictly decreasing, we can pick at most 1 model.

## Input Format
- The first line contains an integer n: the number of models.
- The second line contains n integers x_1, x_2 ... x_n: the RAM of each model in order.

## Output Format
- Return one integer: the length of the longest valid upgrade path.

## Constraints
- 1 ≤ n ≤ 2e5
- 1 ≤ x ≤ 1e9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
binary-search, dynamic-programming, greedy
