## Title

Rainwater Reservoir Capacity

## Slug

rainwater-reservoir-capacity
## Difficulty

Medium

## Description

Imagine a landscape represented by a sequence of vertical bars of varying heights but uniform width (1 unit each). After a heavy rain, water gets trapped between these bars. Your goal is to calculate the total volume of water that can be held in these reservoirs formed by the bars. Assume the ground is flat beneath the bars. 
You are given the heights of n adjacent bars. Calculate the total units of water trapped.

## Examples

### 1

#### Input

12
[0, 1, 0, 2, 1, 0, 1, 3, 2, 1, 2, 1]

#### Output

6

#### Explanation

Total water trapped = 1 + 1 + 2 + 1 + 1 = 6 units.

### 2

#### Input

6
[4, 2, 0, 3, 2, 5]

#### Output

9

#### Explanation

Total water trapped = 2 + 4 + 1 + 2 = 9 units.
  

## Input Format  

- The first line contains a single integer n, the number of bars.
- The second line contains n space-separated non-negative integers, representing the heights of the bars from left to right.

## Output Format  

- Return a single integer representing total units of rainwater trapped.
  

## Constraints  

- 1 ≤ n ≤ 1e5
- 1 ≤ height ≤ 1e9

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

array, two-pointers, stack, dynamic-programming