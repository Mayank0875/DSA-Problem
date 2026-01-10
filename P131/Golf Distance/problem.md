## Title
Golf Distance

## Slug
golf-distance

## Difficulty
Medium

## Description
A golfer hits the ball towards the hole. A magic club hits the ball a distance equal to a digit of the current distance to the pin.

You start with a **distance to pin** of `n`. The goal is to reduce this distance to pin to exactly 0.

In one **stroke**, you can look at the digits of the current distance to pin, choose one **non-zero digit**, and subtract it from the current distance to pin.

For example, if the distance to pin is 27, the digits are 2 and 7. You can subtract 2 (getting 25) or 7 (getting 20).

Your task is to find the **minimum** number of strokes required to reduce the distance to pin to 0.

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
Total strokes: 5.

### 2

#### Input
0

#### Output
0

#### Explanation
The distance to pin is already 0.

## Input Format
- The input contains a single integer `n`.

## Output Format
- Return a single integer representing the minimum number of strokes.

## Constraints
- 0 ≤ n ≤ 10^6

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, greedy, math, bfs
