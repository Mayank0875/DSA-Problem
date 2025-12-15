## Title
Game Health Bar

## Slug
game-health-bar

## Difficulty
Medium

## Description
A boss heals `n` HP. Healing potions give 1 to 6 HP.

Total healing is `n` HP.
Potions are used one after another.

Your task is to calculate the total number of distinct ways to heal the boss such that the total health is exactly `n`. Since the number of possibilities can be astronomical, output the result modulo $10^9 + 7$.

## Examples

### 1

#### Input
8

#### Output
125

#### Explanation
There are 125 distinct sequences.

### 2

#### Input
3

#### Output
4

#### Explanation
There are 4 distinct sequences:
1+1+1
1+2
2+1
3

## Input Format
- The only input line has an integer `n`: the target health.

## Output Format
- Return one integer: the number of ways modulo $10^9 + 7$.

## Constraints
- 1 ≤ n ≤ 10^18

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, maths
