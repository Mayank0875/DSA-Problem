## Title
Escape Room Puzzle

## Slug
escape-room-puzzle

## Difficulty
Hard

## Description
To unlock a door, you must press buttons. You can press the next button or skip one in the sequence.

The player starts at button 0 and wishes to reach button $n$. On each move, The player can press forward either **1 button** or **2 buttons**.

Your task is to calculate the total number of distinct ways to reach exactly button $n$. Since the distance $n$ can be extremely large, return the answer modulo $10^9 + 7$.

## Examples

### 1

#### Input
2

#### Output
2

#### Explanation
There are two ways to reach button 2:
1. 1 button + 1 button
2. 2 buttons

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
- The only input line has an integer $n$ — the target button.

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

