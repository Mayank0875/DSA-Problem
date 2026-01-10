## Title
Mana Drain

## Slug
mana-drain

## Difficulty
Medium

## Description
A wizard is draining mana from a magical crystal. The crystal releases mana in bursts equal to the digits of its current charge level.

You start with a **mana charge** of `n`. The goal is to reduce this mana charge to exactly 0.

In one **drain spell**, you can look at the digits of the current mana charge, choose one **non-zero digit**, and subtract it from the current mana charge.

For example, if the mana charge is 27, the digits are 2 and 7. You can subtract 2 (getting 25) or 7 (getting 20).

Your task is to find the **minimum** number of drain spells required to reduce the mana charge to 0.

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
Total drain spells: 5.

### 2

#### Input
0

#### Output
0

#### Explanation
The mana charge is already 0.

## Input Format
- The input contains a single integer `n`.

## Output Format
- Return a single integer representing the minimum number of drain spells.

## Constraints
- 0 ≤ n ≤ 10^6

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, greedy, math, bfs
