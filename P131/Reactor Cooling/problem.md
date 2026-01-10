## Title
Reactor Cooling

## Slug
reactor-cooling

## Difficulty
Medium

## Description
A nuclear reactor is overheating. To cool it down safely, engineers can reduce the temperature by an amount equal to any non-zero digit of the current temperature.

You start with a **temperature** of `n`. The goal is to reduce this temperature to exactly 0.

In one **cooling cycle**, you can look at the digits of the current temperature, choose one **non-zero digit**, and subtract it from the current temperature.

For example, if the temperature is 27, the digits are 2 and 7. You can subtract 2 (getting 25) or 7 (getting 20).

Your task is to find the **minimum** number of cooling cycles required to reduce the temperature to 0.

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
Total cooling cycles: 5.

### 2

#### Input
0

#### Output
0

#### Explanation
The temperature is already 0.

## Input Format
- The input contains a single integer `n`.

## Output Format
- Return a single integer representing the minimum number of cooling cycles.

## Constraints
- 0 ≤ n ≤ 10^6

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, greedy, math, bfs
