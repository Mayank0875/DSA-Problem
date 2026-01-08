## Title
Heavy Lifter

## Slug
heavy-lifter

## Difficulty
Medium

## Description
A worker stacks boxes. They can lift a light box (1 unit) or a heavy box (2 units). Lifting heavy boxes strains the back, so they can't do two in a row.

The worker starts at height 0 and wants to reach height $n$.

On each move, The worker can lift forward either **1 unit** (+1) or **2 units** (+2). However, stamina is low. Therefore, The worker **cannot perform two consecutive +2 heavy lifts**.

Your task is to calculate the number of distinct valid ways The worker can reach height $n$. Since the answer can be very large, return it modulo $10^9 + 7$.

## Examples

### 1

#### Input
3

#### Output
3

#### Explanation
The valid paths to reach height 3 are:
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
- The only input line has an integer $n$ — the target unit index.

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

