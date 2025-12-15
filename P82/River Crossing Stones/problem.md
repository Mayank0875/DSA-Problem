## Title
River Crossing Stones

## Slug
river-crossing-stones

## Difficulty
Easy

## Description
A frog jumps on n stones. It wants to jump to stones that are progressively further away from the bank.

You have the distances of n stones from the bank.
A valid path consists of stones where each stone is strictly further than the previous one.

You must plan the jumps to find the longest possible crossing path. You can skip any number of stones to form the sequence, but you must maintain the original layout order of the selected stones. Calculate the maximum number of stones that can form such a sequence.

## Examples

### 1

#### Input
8
7 3 5 3 6 2 9 8

#### Output
4

#### Explanation
The input contains: [7, 3, 5, 3, 6, 2, 9, 8]. The longest crossing paths (strictly increasing) include:
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
Since the values are strictly decreasing, we can pick at most 1 stone.

## Input Format
- The first line contains an integer n: the number of stones.
- The second line contains n integers x_1, x_2 ... x_n: the distance of each stone in order.

## Output Format
- Return one integer: the length of the longest valid crossing path.

## Constraints
- 1 ≤ n ≤ 2e5
- 1 ≤ x ≤ 1e9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
binary-search, dynamic-programming, greedy
