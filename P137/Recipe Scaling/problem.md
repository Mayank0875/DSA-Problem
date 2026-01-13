## Title
Recipe Scaling

## Slug
recipe-scaling

## Difficulty
Medium

## Description
A chef has two lists of ingredient quantities for different banquet halls. He needs to scale the quantities so they match exactly for standardization.

You have two lists of ingredient amounts.

In a single scaling step, The chef can:
1. Choose an index $i$ ($1 \le i \le n$).
2. Choose a positive integer $x$.
3. multiply the ingredient quantity value at $i$ in either list by $x$ (i.e., new value = old value $\times x$).

The chef wants to make the lists identical (i.e., $a_i = b_i$ for all $1 \le i \le n$) using the **minimum** number of scaling steps.

Determine the minimum number of scaling steps required to achieve this goal.

## Examples

### 1

#### Input
4
1 2 3 4
7 8 5 3

#### Output
6

#### Explanation
- Index 0: 1 and 7. Multiply 1 by 7 to get 7. (1 op).
- Index 1: 2 and 8. Multiply 2 by 4 to get 8. (1 op).
- Index 2: 3 and 5. Neither divides the other. Multiply 3 by 5 (15) and 5 by 3 (15). (2 ops).
- Index 3: 4 and 3. Neither divides the other. (2 ops).
Total: $1 + 1 + 2 + 2 = 6$.

### 2

#### Input
3
1 5 9
19 2 6

#### Output
5

#### Explanation
- 1 -> 19 (1 op)
- 5 -> 2 (2 ops)
- 9 -> 6 (2 ops)
Total: 5.

## Input Format
- The first line contains an integer $n$.
- The second line contains $n$ integers representing the first list.
- The third line contains $n$ integers representing the second list.

## Output Format
- Return a single integer representing the minimum number of scaling steps.

## Constraints
- 1 ≤ n ≤ 10^5
- 1 ≤ values ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, math, number-theory, greedy
