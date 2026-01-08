## Title
Solar Panel Array

## Slug
solar-panel-array

## Difficulty
Hard

## Description
An installer places panels on a roof. They can place a single panel or a double-width panel.

The installer starts at meter 0 and wishes to reach meter $n$. On each move, The installer can install forward either **1 meter** or **2 meters**.

Your task is to calculate the total number of distinct ways to reach exactly meter $n$. Since the distance $n$ can be extremely large, return the answer modulo $10^9 + 7$.

## Examples

### 1

#### Input
2

#### Output
2

#### Explanation
There are two ways to reach meter 2:
1. 1 meter + 1 meter
2. 2 meters

### 2

#### Input
3

#### Output
3

#### Explanation
There are three ways:
1. 1 + 1 + 1
2. 1 + 2
3. 2 + 1

## Input Format
- The only input line has an integer $n$ — the target meter.

## Output Format
- Return a single integer: the number of ways modulo $10^9 + 7$.

## Constraints
- 1 ≤ n ≤ 10^18

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, math

