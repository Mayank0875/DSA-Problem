## Title
Conveyor Belt Sushi

## Slug
conveyor-belt-sushi

## Difficulty
Hard

## Description
A chef places plates. They can place a small plate (1 slot) or a large platter (2 slots).

The chef starts at slot 0 and wishes to reach slot $n$. On each move, The chef can place forward either **1 slot** or **2 slots**.

Your task is to calculate the total number of distinct ways to reach exactly slot $n$. Since the distance $n$ can be extremely large, return the answer modulo $10^9 + 7$.

## Examples

### 1

#### Input
2

#### Output
2

#### Explanation
There are two ways to reach slot 2:
1. 1 slot + 1 slot
2. 2 slots

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
- The only input line has an integer $n$ — the target slot.

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

