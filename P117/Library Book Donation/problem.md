## Title
Library Book Donation

## Slug
library-book-donation

## Difficulty
Medium

## Description
Books are sorted. The University Library takes the rarest, the Public Library (you) takes the next best, and the Recycler takes the damaged ones.

There are $3n$ books of varying literary value available. The distribution follows a strict protocol. In each round, you must select any 3 books. The parties then claim them based on the following rules:

1. The **University** takes the book with the **maximum** literary value from the triplet.
2. You, the **Public Library**, take the book with the **second maximum** literary value.
3. The **Recycler** takes the remaining book (the one with the minimum literary value).

This process repeats until all books are distributed. Your goal as the Public Library is to maximize the total literary value of the books you acquire.

Given an array of integers `books`, where `books[i]` represents the literary value of the $i$-th book, return the maximum total literary value you can obtain.

## Examples

### 1

#### Input
6
2 4 1 2 7 8

#### Output
9

#### Explanation
You have 6 books. One optimal strategy is:
1. Pick the triplet `(2, 7, 8)`. University takes `8`, you take `7`, Recycler takes `2`.
2. Pick the remaining `(1, 2, 4)`. University takes `4`, you take `2`, Recycler takes `1`.
Total literary value = $7 + 2 = 9$.

### 2

#### Input
3
2 4 5

#### Output
4

#### Explanation
There is only one triplet `(2, 4, 5)`. University takes `5`, you take `4`, Recycler takes `2`. Total = 4.

## Input Format
- The first line contains a single integer $3n$, the number of books.
- The second line contains $3n$ space-separated integers representing the `books` array.

## Output Format
- Return a single integer representing the maximum total literary value you can collect.

## Constraints
- 1 ≤ books.length ≤ 10^5
- `books.length` is divisible by 3.
- 1 ≤ books[i] ≤ 10^4

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, sorting, greedy, math
