## Title

The Celestial Frog

## Slug

the-celestial-frog

## Difficulty

Hard

## Description

A legendary Frog is preparing to travel across the galaxy. The path is a straight line consisting of $n$ star-platforms.

The frog starts at platform 0 and wishes to reach platform $n$. On each move, the frog can jump forward either **1 platform** or **2 platforms**.

Your task is to calculate the total number of distinct ways the frog can reach exactly platform $n$. Since the distance $n$ can be extremely large, return the answer modulo $10^9 + 7$.

## Examples

### 1

#### Input

2

#### Output

2

#### Explanation

There are two ways to reach platform 2:

0 -> 1 -> 2 (1 jump + 1 jump)
0 -> 2 (2 jumps)
    
### 2

#### Input

3

#### Output

3

#### Explanation
There are three ways:

0 -> 1 -> 2 -> 3
0 -> 1 -> 3
0 -> 2 -> 3
  

## Input Format  

- The only input line has an integer n — the target platform..

## Output Format  

- Return a single integer: the number of ways modulo $10^9 + 7$.
  

## Constraints  

- 1 ≤ n ≤ 1e18

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

dynamic-programming, math

## Company
tiktok