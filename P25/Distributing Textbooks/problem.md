## Title

Distributing Textbooks

## Slug

distributing-textbooks

## Difficulty

Medium

## Description

A school has `n` stacks of textbooks to give out, lined up in order. Stack `i` has `x[i]` books. There are `k` classrooms. Each classroom must receive a contiguous block of stacks (e.g., room 1 gets stacks 1-3, room 2 gets stacks 4-5, etc.). What is the minimum possible value for the maximum number of books any single classroom receives?

## Examples

### 1

#### Input

5 3 
2 4 7 3 5


#### Output

8

#### Explanation

An optimal distribution assigns scrolls [2, 4] to the first scribe (sum 6 pages), scroll [7] to the second scribe (sum 7 pages), and scrolls [3, 5] to the third scribe (sum 8 pages). The maximum number of pages assigned to any scribe is 8. No other distribution into 3 contiguous blocks can achieve a maximum load less than 8.

### 2

#### Input

1 1
34

#### Output

34


#### Explanation

No other distribution into 1 contiguous blocks can achieve a maximum load less than 34.

## Input Format

- The first line contains two integers `n` and `k`: the number of stacks and the number of classrooms.
- The second line contains `n` integers `x[1], x[2] ... x[n]`, where `x[i]` is the number of books in the i-th stack.

## Output Format

- Return one integer: the minimum possible value for the maximum number of pages assigned to any scribe.

## Constraints

- 1 ≤ k ≤ n ≤ 2e5
- 1 ≤ x[i] ≤ 10^9

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

binary-search, greedy