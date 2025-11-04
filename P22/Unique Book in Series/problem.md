## Title

Unique Book in Series

## Slug

unique-book-in-series

## Difficulty

Medium

## Description

A library shelf is sorted by book ID. All books are part of a two-volume set, so their IDs appear twice. For example, `[10, 10, 20, 20]`. However, one book on the shelf is a standalone story and its ID appears only once. Given the sorted list of `n` book IDs, find the ID of the standalone book.

You must write an algorithm with O(log n) runtime complexity.

## Examples

### 1

#### Input

9 
[1, 1, 2, 3, 3, 4, 4, 8, 8]


#### Output

2

#### Explanation

In the sequence [1, 1, 2, 3, 3, 4, 4, 8, 8], the number 2 appears only once.

### 2

#### Input

7 
[3, 3, 7, 7, 10, 11, 11]

#### Output

10

#### Explanation

In the sequence [3, 3, 7, 7, 10, 11, 11], the number 10 appears only once.

## Input Format

- The first line contains an odd integer n, the total number of books.
- The second line contains n space-separated integers representing the sorted book IDs.

## Output Format

- Return a single integer: the ID of the book that appears only once.

## Constraints

- 1 ≤ n ≤ 10^5
- 1 ≤ stone_value ≤ 10^9
- The array is sorted.
- Every element appears twice except for one.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

binary-search, array