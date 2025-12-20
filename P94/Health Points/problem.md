## Title
Health Points

## Slug
health-points

## Difficulty
Easy

## Description
You are fighting a boss with regenerative armor. Your attacks deal damage equal to any digit in the boss's current HP.

The boss HP currently has a value of $n$. To defeat the boss, you must reduce this value exactly to $0$.

The mechanism works as follows: in a single step, you can decrease the current value by subtracting **any one of the digits** present in the number itself.
For example, if the value is $27$, you can subtract $2$ (becoming $25$) or $7$ (becoming $20$).

Your task is to determine the **minimum** number of steps required to reduce the value from $n$ to $0$.

## Examples

### 1

#### Input
27

#### Output
5

#### Explanation
Total steps: 5.
One optimal path: 27 -> 20 -> 18 -> 10 -> 9 -> 0.

### 2

#### Input
17

#### Output
3

#### Explanation
Total steps: 3.
Path: 17 -> 10 -> 9 -> 0.

## Input Format
- The only input line has an integer $n$.

## Output Format
- Return one integer: the minimum number of steps to reach 0.

## Constraints
- 1 ≤ n ≤ 10^6

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, math, greedy
