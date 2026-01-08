## Title
Subway Stations

## Slug
subway-stations

## Difficulty
Hard

## Description
An express train moves down the line. It can stop at the next station or skip one to stop at the second.

The train starts at station 0 and wishes to reach station $n$. On each move, The train can travel forward either **1 station** or **2 stations**.

Your task is to calculate the total number of distinct ways to reach exactly station $n$. Since the distance $n$ can be extremely large, return the answer modulo $10^9 + 7$.

## Examples

### 1

#### Input
2

#### Output
2

#### Explanation
There are two ways to reach station 2:
1. 1 station + 1 station
2. 2 stations

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
- The only input line has an integer $n$ — the target station.

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

