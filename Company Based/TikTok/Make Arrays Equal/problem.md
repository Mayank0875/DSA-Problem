## Title

Make Arrays Equal

## Slug

make-arrays-equal

## Difficulty

Medium

## Description

Alex wants to impress Alice by making two integer arrays, $a$ and $b$, equal. Both arrays currently contain $n$ elements.

In a single operation, Alex can perform the following:
1. Choose an index $i$ ($1 \le i \le n$).
2. Choose a positive integer $x$.
3. Multiply either $a_i$ or $b_i$ by $x$.

Alex wants to make the arrays identical (i.e., $a_i = b_i$ for all $1 \le i \le n$) using the minimum number of operations.

Determine the minimum number of operations required to achieve this goal.

## Examples

### 1

#### Input

4
1 2 3 4
7 8 5 3

#### Output

6

#### Explanation

- $a_0=1, b_0=7$. $1 \times 7 = 7$. (1 op).
- $a_1=2, b_1=8$. $2 \times 4 = 8$. (1 op).
- $a_2=3, b_2=5$. Neither divides the other. Multiply $a_2$ by 5 (15) and $b_2$ by 3 (15). (2 ops).
- $a_3=4, b_3=3$. Neither divides the other. (2 ops).
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
- The second line contains $n$ integers representing array $a$.
- The third line contains $n$ integers representing array $b$.

## Output Format  

- Return a single integer representing the minimum number of operations.  

## Constraints  

- 1 ≤ n ≤ 1e5
- 1 ≤ a[i], b[i] ≤ 1e5


## Time Limit

2 second

## Memory Limit

256 MB

## Tags

array, math, number-theory