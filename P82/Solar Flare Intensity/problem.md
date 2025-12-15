## Title
Solar Flare Intensity

## Slug
solar-flare-intensity

## Difficulty
Easy

## Description
An observatory records n flares. A solar storm warning is triggered by a sequence of strictly intensifying flares.

You have intensity readings for n flares.
A storm warning consists of flares where intensity is strictly higher than the previous flare.

You must issue warning to find the longest possible storm sequence. You can skip any number of flares to form the sequence, but you must maintain the original time order of the selected flares. Calculate the maximum number of flares that can form such a sequence.

## Examples

### 1

#### Input
8
7 3 5 3 6 2 9 8

#### Output
4

#### Explanation
The input contains: [7, 3, 5, 3, 6, 2, 9, 8]. The longest storm sequences (strictly increasing) include:
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
Since the values are strictly decreasing, we can pick at most 1 flare.

## Input Format
- The first line contains an integer n: the number of flares.
- The second line contains n integers x_1, x_2 ... x_n: the intensity of each flare in order.

## Output Format
- Return one integer: the length of the longest valid storm sequence.

## Constraints
- 1 ≤ n ≤ 2e5
- 1 ≤ x ≤ 1e9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
binary-search, dynamic-programming, greedy
