## Title
Piano Tiles Game

## Slug
piano-tiles-game

## Difficulty
Hard

## Description
A player taps tiles on a screen. Tiles appear singly or as double-length holds.

The player starts at beat 0 and wishes to reach beat $n$. On each move, The player can tap forward either **1 beat** or **2 beats**.

Your task is to calculate the total number of distinct ways to reach exactly beat $n$. Since the distance $n$ can be extremely large, return the answer modulo $10^9 + 7$.

## Examples

### 1

#### Input
2

#### Output
2

#### Explanation
There are two ways to reach beat 2:
1. 1 beat + 1 beat
2. 2 beats

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
- The only input line has an integer $n$ — the target beat.

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

