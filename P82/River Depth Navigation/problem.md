## Title
River Depth Navigation

## Slug
river-depth-navigation

## Difficulty
Easy

## Description
A submarine navigates a trench with varying depths. It must move deeper at each checkpoint to avoid turbulence.

You have depth readings for n checkpoints.
A safe path consists of checkpoints where the depth is strictly greater than the previous checkpoint.

You must chart the course to find the longest possible descent path. You can skip any number of checkpoints to form the sequence, but you must maintain the original travel order of the selected checkpoints. Calculate the maximum number of checkpoints that can form such a sequence.

## Examples

### 1

#### Input
8
7 3 5 3 6 2 9 8

#### Output
4

#### Explanation
The input contains: [7, 3, 5, 3, 6, 2, 9, 8]. The longest descent paths (strictly increasing) include:
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
Since the values are strictly decreasing, we can pick at most 1 checkpoint.

## Input Format
- The first line contains an integer n: the number of checkpoints.
- The second line contains n integers x_1, x_2 ... x_n: the depth of each checkpoint in order.

## Output Format
- Return one integer: the length of the longest valid descent path.

## Constraints
- 1 ≤ n ≤ 2e5
- 1 ≤ x ≤ 1e9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
binary-search, dynamic-programming, greedy
