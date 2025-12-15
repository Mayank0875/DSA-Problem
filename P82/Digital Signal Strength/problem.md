## Title
Digital Signal Strength

## Slug
digital-signal-strength

## Difficulty
Easy

## Description
A receiver logs signal strength over time. To lock onto a satellite, the system needs a sequence of increasing signal pulses.

You have n signal strength values.
A lock sequence consists of pulses where each pulse is strictly stronger than the previous one.

You must process the log to find the longest possible lock sequence. You can skip any number of pulses to form the sequence, but you must maintain the original time order of the selected pulses. Calculate the maximum number of pulses that can form such a sequence.

## Examples

### 1

#### Input
8
7 3 5 3 6 2 9 8

#### Output
4

#### Explanation
The input contains: [7, 3, 5, 3, 6, 2, 9, 8]. The longest lock sequences (strictly increasing) include:
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
Since the values are strictly decreasing, we can pick at most 1 pulse.

## Input Format
- The first line contains an integer n: the number of pulses.
- The second line contains n integers x_1, x_2 ... x_n: the strength of each pulse in order.

## Output Format
- Return one integer: the length of the longest valid lock sequence.

## Constraints
- 1 ≤ n ≤ 2e5
- 1 ≤ x ≤ 1e9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
binary-search, dynamic-programming, greedy
