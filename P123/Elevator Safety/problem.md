## Title
Elevator Safety

## Slug
elevator-safety

## Difficulty
Medium

## Description
A service elevator moves floors. It can go up 1 floor or skip to go up 2 floors. Skipping floors vibrates the cable, so it cannot be done twice in a row.

The elevator starts at floor 0 and wants to reach floor $n$.

On each move, The elevator can move forward either **1 floor** (+1) or **2 floors** (+2). However, safety sensors trigger. Therefore, The elevator **cannot perform two consecutive +2 skips**.

Your task is to calculate the number of distinct valid ways The elevator can reach floor $n$. Since the answer can be very large, return it modulo $10^9 + 7$.

## Examples

### 1

#### Input
3

#### Output
3

#### Explanation
The valid paths to reach floor 3 are:
1. 0 -> 1 -> 2 -> 3 (+1, +1, +1)
2. 0 -> 1 -> 3 (+1, +2)
3. 0 -> 2 -> 3 (+2, +1)

Note: The path starting with +2 is valid as long as the next jump is not +2.

### 2

#### Input
4

#### Output
4

#### Explanation
Valid paths:
1. 0 -> 1 -> 2 -> 3 -> 4 (+1, +1, +1, +1)
2. 0 -> 1 -> 2 -> 4 (+1, +1, +2)
3. 0 -> 1 -> 3 -> 4 (+1, +2, +1)
4. 0 -> 2 -> 3 -> 4 (+2, +1, +1)

Invalid path:
0 -> 2 -> 4 (+2, +2) is not allowed.

## Input Format
- The only input line has an integer $n$ — the target floor index.

## Output Format
- Return a single integer: the number of ways modulo $10^9 + 7$.

## Constraints
- 1 ≤ n ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, math

