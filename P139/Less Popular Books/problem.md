## Title
Less Popular Books

## Slug
less-popular-books

## Difficulty
Medium

## Description
A publisher analyzes book sales.

You have a list of $n$ books. Each book has two main properties: **review rating** and **sales count**. You are given a 2D integer array `properties` where `properties[i] = [review rating_i, sales count_i]` represents the attributes of the $i$-th book.

A book is considered **less popular** if there exists another book that has **both** strictly greater review rating and strictly greater sales count.

More formally, the $i$-th book is less popular if there exists an index $j$ such that `review rating_j > review rating_i` and `sales count_j > sales count_i`.

Your task is to return the number of less popular books.

## Examples

### 1

#### Input
3
5 5
6 3
3 6

#### Output
0

#### Explanation
No book has strictly greater review rating and sales count than another.

### 2

#### Input
2
2 2
3 3

#### Output
1

#### Explanation
The first book (2, 2) is less popular because the second book (3, 3) has strictly greater review rating and sales count.

## Input Format
- The first line contains an integer $n$, the number of books.
- The next $n$ lines each contain two space-separated integers, representing the review rating and sales count of a book.

## Output Format
- Return a single integer representing the number of less popular books.

## Constraints
- 1 ≤ n ≤ 10^5
- 1 ≤ review rating, sales count ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, greedy, sorting
