## Title
Ocean Wave Height

## Slug
ocean-wave-height

## Difficulty
Easy

## Description
A buoy measures n waves. A rogue wave build-up is a sequence of strictly increasing wave heights.

You have heights for n waves.
A build-up consists of waves where height is strictly higher than the previous wave.

You must monitor the sea to find the longest possible rogue build-up. You can skip any number of waves to form the sequence, but you must maintain the original time order of the selected waves. Calculate the maximum number of waves that can form such a sequence.

## Examples

### 1

#### Input
8
7 3 5 3 6 2 9 8

#### Output
4

#### Explanation
The input contains: [7, 3, 5, 3, 6, 2, 9, 8]. The longest rogue build-ups (strictly increasing) include:
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
Since the values are strictly decreasing, we can pick at most 1 wave.

## Input Format
- The first line contains an integer n: the number of waves.
- The second line contains n integers x_1, x_2 ... x_n: the height of each wave in order.

## Output Format
- Return one integer: the length of the longest valid rogue build-up.

## Constraints
- 1 ≤ n ≤ 2e5
- 1 ≤ x ≤ 1e9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
binary-search, dynamic-programming, greedy
