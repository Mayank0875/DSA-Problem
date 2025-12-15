## Title
Marathon Pace

## Slug
marathon-pace

## Difficulty
Easy

## Description
A runner logs splits for n miles. They want to find a negative split strategy where speed strictly increases.

You have speed values for n miles.
A negative split strategy consists of miles where speed is strictly higher than the previous mile.

You must review the race to find the longest possible pacing strategy. You can skip any number of miles to form the sequence, but you must maintain the original distance order of the selected miles. Calculate the maximum number of miles that can form such a sequence.

## Examples

### 1

#### Input
8
7 3 5 3 6 2 9 8

#### Output
4

#### Explanation
The input contains: [7, 3, 5, 3, 6, 2, 9, 8]. The longest pacing strategys (strictly increasing) include:
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
Since the values are strictly decreasing, we can pick at most 1 mile.

## Input Format
- The first line contains an integer n: the number of miles.
- The second line contains n integers x_1, x_2 ... x_n: the speed of each mile in order.

## Output Format
- Return one integer: the length of the longest valid pacing strategy.

## Constraints
- 1 ≤ n ≤ 2e5
- 1 ≤ x ≤ 1e9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
binary-search, dynamic-programming, greedy
