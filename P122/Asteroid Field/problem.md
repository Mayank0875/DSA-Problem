## Title
Asteroid Field

## Slug
asteroid-field

## Difficulty
Hard

## Description
A spaceship dodges rocks. It can maneuver past 1 rock or barrel roll past 2.

The pilot starts at sector 0 and wishes to reach sector $n$. On each move, The pilot can fly forward either **1 sector** or **2 sectors**.

Your task is to calculate the total number of distinct ways to reach exactly sector $n$. Since the distance $n$ can be extremely large, return the answer modulo $10^9 + 7$.

## Examples

### 1

#### Input
2

#### Output
2

#### Explanation
There are two ways to reach sector 2:
1. 1 sector + 1 sector
2. 2 sectors

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
- The only input line has an integer $n$ — the target sector.

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

