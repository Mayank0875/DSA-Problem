## Title

The Alchemist's Fusion

## Slug

the-alchemists-fusion

## Difficulty

Medium

## Description

Elias is a renowned alchemist working on creating the ultimate magical artifact. He has a collection of $n$ elemental stones, where the $i$-th stone has a power level of $a_i$.

According to the ancient texts, a "Perfect Fusion" occurs when two stones interact to form a combined power that is a perfect $k$-th power. Mathematically, two stones with power levels $a_i$ and $a_j$ (where $1 \le i < j \le n$) form a Perfect Fusion if there exists an integer $x$ such that:
$$a_i \cdot a_j = x^k$$

Elias needs to know how many such pairs exist in his collection to prepare his laboratory. Your task is to count the number of pairs $(i, j)$ with $1 \le i < j \le n$ that satisfy this condition.

## Examples

### 1

#### Input

6 3
1 3 9 8 24 1

#### Output

5

#### Explanation

The suitable pairs are:
- $1 \cdot 8 = 8 = 2^3$
- $1 \cdot 1 = 1 = 1^3$
- $3 \cdot 9 = 27 = 3^3$
- $9 \cdot 24 = 216 = 6^3$
- $8 \cdot 1 = 8 = 2^3$
    
### 2

#### Input

4 2
4 4 4 4

#### Output

6

#### Explanation

$4 \cdot 4 = 16 = 4^2$. All pairs work. The number of pairs is $\frac{4 \times 3}{2} = 6$.
  

## Input Format  

- The first line contains two integers $n$ and $k$ ($2 \le n \le 10^5$, $2 \le k \le 100$).
- The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^5$).

## Output Format  

- Return one integer: the number of suitable pairs.
  

## Constraints  

- 1 ≤ n ≤ 1e5
- 1 ≤ k ≤ 100
- 1 ≤ a_i ≤ 1e5

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

array, math, number-theory, dynamic-programming