## Title
Volcanic Pressure

## Slug
volcanic-pressure

## Difficulty
Easy

## Description
A sensor logs n pressure events. A geophysicist looks for a buildup sequence leading to eruption.

You have n pressure readings.
A buildup sequence consists of readings where pressure is strictly higher than the previous reading.

You must monitor the volcano to find the longest possible buildup sequence. You can skip any number of readings to form the sequence, but you must maintain the original time order of the selected readings. Calculate the maximum number of readings that can form such a sequence.

## Examples

### 1

#### Input
8
7 3 5 3 6 2 9 8

#### Output
4

#### Explanation
The input contains: [7, 3, 5, 3, 6, 2, 9, 8]. The longest buildup sequences (strictly increasing) include:
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
Since the values are strictly decreasing, we can pick at most 1 reading.

## Input Format
- The first line contains an integer n: the number of readings.
- The second line contains n integers x_1, x_2 ... x_n: the pressure of each reading in order.

## Output Format
- Return one integer: the length of the longest valid buildup sequence.

## Constraints
- 1 ≤ n ≤ 2e5
- 1 ≤ x ≤ 1e9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
binary-search, dynamic-programming, greedy
