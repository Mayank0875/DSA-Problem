## Title
Solar Energy

## Slug
solar-energy

## Difficulty
Easy

## Description
A homeowner with a battery tracks grid buy-back rates. They store energy (buy) when it's cheap and sell to the grid when rates are high.

You have a list of energy rate for $n$ consecutive hours. You want to make one perfect move: charge on one hour and discharge on a different hour in the future. You cannot discharge before you charge.

Your goal is to find the **maximum possible credit** you can earn from this single transaction. If it is impossible to make any credit (i.e., the energy rate only goes down), you should return 0.

## Examples

### 1

#### Input
6
7 1 5 3 6 4

#### Output
5

#### Explanation
charge on hour 2 (energy rate = 1) and discharge on hour 5 (energy rate = 6). The credit is $6 - 1 = 5$.
Note that chargeing on hour 1 (energy rate = 7) is not optimal, as all future values are lower.

### 2

#### Input
5
7 6 4 3 1

#### Output
0

#### Explanation
The energy rate never increases, so it is impossible to make a credit. The maximum credit is 0.

## Input Format
- The first line contains a single integer `n`, the number of hours.
- The second line contains `n` space-separated integers representing the energy rate on each hour.

## Output Format
- Return a single integer representing the maximum credit. If no credit can be made, return 0.

## Constraints
- 1 ≤ n ≤ 10^5
- 0 ≤ values ≤ 10^4

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, dynamic-programming, greedy
