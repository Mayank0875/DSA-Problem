## Title
Sprinter Splits

## Slug
sprinter-splits

## Difficulty
Easy

## Description
A coach analyzes n split times. They want to find a sequence where the runner strictly increased their speed (decreased split time, logic inverted for LIS context: assume 'speed' value increases).

You have speed values for n splits.
A acceleration phase consists of splits where speed is strictly higher than the previous split.

You must analyze performance to find the longest possible acceleration phase. You can skip any number of splits to form the sequence, but you must maintain the original race order order of the selected splits. Calculate the maximum number of splits that can form such a sequence.

## Examples

### 1

#### Input
8
7 3 5 3 6 2 9 8

#### Output
4

#### Explanation
The input contains: [7, 3, 5, 3, 6, 2, 9, 8]. The longest acceleration phases (strictly increasing) include:
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
Since the values are strictly decreasing, we can pick at most 1 split.

## Input Format
- The first line contains an integer n: the number of splits.
- The second line contains n integers x_1, x_2 ... x_n: the speed of each split in order.

## Output Format
- Return one integer: the length of the longest valid acceleration phase.

## Constraints
- 1 ≤ n ≤ 2e5
- 1 ≤ x ≤ 1e9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
binary-search, dynamic-programming, greedy
