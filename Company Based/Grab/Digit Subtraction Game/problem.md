## Title

Digit Subtraction Game

## Slug

digit-subtraction-game

## Difficulty

Medium

## Description

You are given an integer `num`. You need to reduce this number to 0.

In one step, you can look at the digits of the current number, choose one non-zero digit, and subtract it from the number.

For example, if the number is 27, the digits are 2 and 7. You can subtract 2 (getting 25) or 7 (getting 20).

Your task is to find the **minimum** number of steps required to reduce the given integer `num` to 0.

## Examples

### 1

#### Input

27

#### Output

5

#### Explanation

1. 27 - 7 = 20
2. 20 - 2 = 18
3. 18 - 8 = 10
4. 10 - 1 = 9
5. 9 - 9 = 0
Total steps: 5.
    
### 2

#### Input

0

#### Output

0

#### Explanation

The number is already 0.

## Input Format  

- The input contains a single integer `num`.

## Output Format  

- Return a single integer representing the minimum number of steps.
  

## Constraints  

- 1 ≤ nums ≤ 1e6

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

dynamic-programming, greedy, math