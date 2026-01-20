## Title

The Dual-Essence Stones

## Slug

the-dual-essence-stones

## Difficulty

Medium

## Description

In the mystical city of Arcanum, there exists a rare type of gem known as a "Dual-Essence Stone". The local alchemists believe that these stones are the most stable because they contain energy from exactly two distinct elemental sources.

The magical properties of a stone are determined by its numeric identifier, $X$. A number is considered to represent a Dual-Essence Stone (or a PQ-prime number) if it has exactly **two distinct prime divisors**.

Mathematically, a number $X$ is a Dual-Essence Stone if it can be represented as:
$$X = P^{K_1} \times Q^{K_2}$$
where $P$ and $Q$ are distinct prime numbers, and $K_1, K_2 \ge 1$.

For example:
* $6 = 2^1 \times 3^1$ is a Dual-Essence Stone (primes 2 and 3).
* $12 = 2^2 \times 3^1$ is a Dual-Essence Stone (primes 2 and 3).
* $8 = 2^3$ is **not** (only prime 2).
* $30 = 2 \times 3 \times 5$ is **not** (three distinct primes).

The Grand Alchemist has given you a range of integers from 1 to $n$. Your task is to count how many numbers in this range represent Dual-Essence Stones.

## Examples

### 1

#### Input

6

#### Output

1

#### Explanation

Between 1 and 6:
- 1: 0 prime factors
- 2: 1 prime factor (2)
- 3: 1 prime factor (3)
- 4: 1 prime factor (2)
- 5: 1 prime factor (5)
- 6: 2 prime factors (2, 3) -> **YES**
Total count is 1.
    
### 2

#### Input

12

#### Output

3

#### Explanation

The Dual-Essence Stones up to 12 are:
- 6 ($2 \times 3$)
- 10 ($2 \times 5$)
- 12 ($2^2 \times 3$)
  

## Input Format  

- The only input line has an integer n.

## Output Format  

- Return a single integer representing the count of numbers between 1 and $n$ (inclusive) that have exactly two distinct prime factors.
  

## Constraints  

- 1 ≤ n ≤ 3000

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

binary-search, math, number-theory

## Company
google