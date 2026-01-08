## Title
Book Pagination

## Slug
book-pagination

## Difficulty
Hard

## Description
A typesetter lays out pages. They can fit text on 1 page or a 2-page spread.

The typesetter starts at page 0 and wishes to reach page $n$. On each move, The typesetter can layout forward either **1 page** or **2 pages**.

Your task is to calculate the total number of distinct ways to reach exactly page $n$. Since the distance $n$ can be extremely large, return the answer modulo $10^9 + 7$.

## Examples

### 1

#### Input
2

#### Output
2

#### Explanation
There are two ways to reach page 2:
1. 1 page + 1 page
2. 2 pages

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
- The only input line has an integer $n$ — the target page.

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

