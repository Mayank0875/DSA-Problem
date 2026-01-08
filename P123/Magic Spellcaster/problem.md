## Title
Magic Spellcaster

## Slug
magic-spellcaster

## Difficulty
Medium

## Description
A wizard duels using mana. They can cast a minor spell (1 mana) or a major spell (2 mana). Major spells destabilize the ether, preventing consecutive major casts.

The wizard starts at power level 0 and wants to reach power level $n$.

On each move, The wizard can cast forward either **1 level** (+1) or **2 levels** (+2). However, the magical field becomes unstable. Therefore, The wizard **cannot perform two consecutive +2 major casts**.

Your task is to calculate the number of distinct valid ways The wizard can reach power level $n$. Since the answer can be very large, return it modulo $10^9 + 7$.

## Examples

### 1

#### Input
3

#### Output
3

#### Explanation
The valid paths to reach power level 3 are:
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
- The only input line has an integer $n$ — the target level index.

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

