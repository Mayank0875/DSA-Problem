## Title

The Cautious Frog

## Slug

the-cautious-frog

## Difficulty

Medium

## Description

A frog is traveling across a pond that consists of $n$ lily pads arranged in a straight line, indexed from 0 to $n$. The frog starts at index 0 and wants to reach index $n$.

On each move, the frog can jump forward either **1 pad** (+1) or **2 pads** (+2). However, this frog is cautious and tires easily after a large jump. Therefore, it **cannot perform two consecutive +2 jumps**.

Your task is to calculate the number of distinct valid ways the frog can reach pad $n$. Since the answer can be very large, return it modulo $10^9 + 7$.

## Examples

### 1

#### Input

3

#### Output

3

#### Explanation

The valid paths to reach pad 3 are:
1. $0 \to 1 \to 2 \to 3$ (+1, +1, +1)
2. $0 \to 1 \to 3$ (+1, +2)
3. $0 \to 2 \to 3$ (+2, +1)
Note: The path $0 \to 2 \to \dots$ (starting with +2) is valid as long as the next jump is not +2.
    
### 2

#### Input

4

#### Output

4

#### Explanation

Valid paths:
1. $0 \to 1 \to 2 \to 3 \to 4$ (+1, +1, +1, +1)
2. $0 \to 1 \to 2 \to 4$ (+1, +1, +2)
3. $0 \to 1 \to 3 \to 4$ (+1, +2, +1)
4. $0 \to 2 \to 3 \to 4$ (+2, +1, +1)
Invalid path: $0 \to 2 \to 4$ (+2, +2) is not allowed.
  

## Input Format  

- The only input line has an integer n — the target lily pad index.

## Output Format  

- Return a single integer: the number of ways modulo $10^9 + 7$.
  

## Constraints  

- 1 ≤ n ≤ 1e5

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

dynamic-programming, math