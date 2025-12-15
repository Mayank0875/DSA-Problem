## Title
Rocket Staging

## Slug
rocket-staging

## Difficulty
Easy

## Description
A rocket has n potential stages. Each active stage must provide strictly more thrust than the previous one.

You have thrust values for n stages.
A valid configuration consists of stages where thrust is strictly higher than the previous stage.

You must configure the rocket to find the longest possible thrust configuration. You can skip any number of stages to form the sequence, but you must maintain the original stack order order of the selected stages. Calculate the maximum number of stages that can form such a sequence.

## Examples

### 1

#### Input
8
7 3 5 3 6 2 9 8

#### Output
4

#### Explanation
The input contains: [7, 3, 5, 3, 6, 2, 9, 8]. The longest thrust configurations (strictly increasing) include:
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
Since the values are strictly decreasing, we can pick at most 1 stage.

## Input Format
- The first line contains an integer n: the number of stages.
- The second line contains n integers x_1, x_2 ... x_n: the thrust of each stage in order.

## Output Format
- Return one integer: the length of the longest valid thrust configuration.

## Constraints
- 1 ≤ n ≤ 2e5
- 1 ≤ x ≤ 1e9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
binary-search, dynamic-programming, greedy
