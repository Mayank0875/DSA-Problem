## Title

Flooded Valley Simulation

## Slug

flooded-valley-simulation
## Difficulty

Medium

## Description

After a long monsoon, several valleys formed between uneven mountain ridges.
Each ridge is represented by a vertical bar of height h[i], and every bar has the same width of one unit.
When it rains, water gets trapped in these valleys.
Your task is to calculate the total amount of rainwater that can be stored between these ridges.

You are given an array representing the heights of the ridges from left to right.
Find the total number of water units trapped after the rainfall.

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