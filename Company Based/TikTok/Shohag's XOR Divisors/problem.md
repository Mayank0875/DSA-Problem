## Title

Shohag's XOR Divisors

## Slug

shohags-xor-divisors

## Difficulty

Medium

## Description

Shohag is fascinated by the interactions between bitwise operations and divisibility. He recently discovered a curious relationship between a fixed integer $x$ and other integers $y$.

He calls an integer $y$ "compatible" with $x$ if the following conditions are met:
1. $y$ is a positive integer such that $1 \le y \le m$.
2. $y \neq x$.
3. The value $(x \oplus y)$ is a divisor of $x$ **OR** $(x \oplus y)$ is a divisor of $y$.

Here, $\oplus$ denotes the bitwise XOR operation. An integer $b$ is a divisor of $a$ if $a$ is divisible by $b$ (i.e., $a \% b = 0$).

Given $x$ and $m$, help Shohag count the total number of suitable integers $y$.

## Examples

### 1

#### Input

6 9

#### Output

3

#### Explanation

In the first test case ($x=6, m=9$):
- For $y=4$: $x \oplus y = 6 \oplus 4 = 2$. $2$ divides $6$. Valid.
- For $y=5$: $x \oplus y = 6 \oplus 5 = 3$. $3$ divides $6$. Valid.
- For $y=7$: $x \oplus y = 6 \oplus 7 = 1$. $1$ divides $6$ (and $7$). Valid.
Total valid values: 3.
    
### 2

#### Input

5 7

#### Output

2

#### Explanation

In the this test case, for 𝑥=5, there are 2valid values for 𝑦among the integers from 1 to 𝑚=7, and they are 4 and 6.

𝑦=4 is valid because 𝑥⊕𝑦=5⊕4=1 and 1 is a divisor of both 𝑥=5 and 𝑦=4.
𝑦=6 is valid because 𝑥⊕𝑦=5⊕6=3 and 3 is a divisor of 𝑦=6.

  

## Input Format  

- Single line containing two space-separated integers $x$ and $m$.

## Output Format  

Return a single integer — the number of suitable $y$.
  

## Constraints  

- 1 ≤ x ≤ 1e6
- 1 ≤ m ≤ 1e18

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

math, number-theory