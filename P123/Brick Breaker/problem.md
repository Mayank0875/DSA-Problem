## Title
Brick Breaker

## Slug
brick-breaker

## Difficulty
Medium

## Description
A ball hits bricks. It can break a standard brick (1 point) or a reinforced brick (2 points). Reinforced bricks slow the ball, preventing it from breaking another heavy one immediately.

The ball starts at score 0 and wants to reach score $n$.

On each move, The ball can break forward either **1 point** (+1) or **2 points** (+2). However, momentum is reduced. Therefore, The ball **cannot perform two consecutive +2 heavy breaks**.

Your task is to calculate the number of distinct valid ways The ball can reach score $n$. Since the answer can be very large, return it modulo $10^9 + 7$.

## Examples

### 1

#### Input
3

#### Output
3

#### Explanation
The valid paths to reach score 3 are:
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
- The only input line has an integer $n$ — the target point index.

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

