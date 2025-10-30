## Title

Festival Light Synchronization

## Slug

festival-light-synchronization

## Difficulty

Medium

## Description

You are setting up N strings of festival lights. Each string `i` is programmed to blink every `A[i]` milliseconds. To create a pleasant effect, you want all strings to blink based on a common time divisor. You can replace exactly one light string with a new one, which can be set to any blink frequency from 1 to 10⁹ ms. What is the maximum possible common frequency (GCD) you can set for all N strings?

## Examples

### 1

#### Input

3 
[7, 6, 8]

#### Output

2

#### Explanation

If you replace the 7ms string with a 4ms string, the frequencies [4, 6, 8] all share a common divisor of 2.

### 2

#### Input

2
[100, 100]

#### Output

100

#### Explanation

You can replace a 100ms string with another 100ms string.

## Input Format

- First line: integer 'n' representing the number of elements written on the blackboard .  
- Second line: 'n' integers representing the elements that are written on blackboard.
- You will be given the array as an input to your function

## Output Format

- Return an integer representing the greatest common divisor after making your move.

## Constraints

- 1 ≤ n ≤ 10^5
- 1 ≤ arr[i] ≤ 10^9

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

arrays, prefix sum, suffix sum, math