## Title
Rollercoaster G-Force

## Slug
rollercoaster-g-force

## Difficulty
Easy

## Description
A designer checks n track segments. They want to ensure a sequence of strictly increasing thrills (G-force).

You have G-force ratings for n segments.
A thrill sequence consists of segments where the G-force is strictly higher than the previous segment.

You must design the track to find the longest possible thrill sequence. You can skip any number of segments to form the sequence, but you must maintain the original track order order of the selected segments. Calculate the maximum number of segments that can form such a sequence.

## Examples

### 1

#### Input
8
7 3 5 3 6 2 9 8

#### Output
4

#### Explanation
The input contains: [7, 3, 5, 3, 6, 2, 9, 8]. The longest thrill sequences (strictly increasing) include:
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
Since the values are strictly decreasing, we can pick at most 1 segment.

## Input Format
- The first line contains an integer n: the number of segments.
- The second line contains n integers x_1, x_2 ... x_n: the G-force of each segment in order.

## Output Format
- Return one integer: the length of the longest valid thrill sequence.

## Constraints
- 1 ≤ n ≤ 2e5
- 1 ≤ x ≤ 1e9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
binary-search, dynamic-programming, greedy
