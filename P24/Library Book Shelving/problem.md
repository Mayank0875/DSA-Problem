## Title

Library Book Shelving

## Slug

library-book-shelving

## Difficulty

Easy

## Description

You are a librarian managing a shelf of books sorted by their Dewey Decimal number (represented as integers). A new book arrives with a specific ID, and you need to place it on the shelf while keeping it sorted.

Your task is to determine the index where this new book should be inserted.
The index should point to the first book that has an ID greater than or equal to the new book's ID.
If all existing books have smaller IDs, the book should be placed at the end of the shelf.


## Examples

### 1

#### Input

6 8
[2, 5, 7, 8, 11, 12]


#### Output

3

#### Explanation

The first product with an ID greater than or equal to 8 is at index 3.

### 2

#### Input

6 6
[2, 5, 7, 8, 11, 12]

#### Output

2

#### Explanation

No product has an ID equal to 6.
The first product with a larger ID (7) appears at index 2.

## Input Format

- The first line contains two integers n and target, where n = number of product IDs, and target = ID of the new product.
- The second line contains n space-separated integers — the sorted list of product IDs.

## Output Format

- Return a single integer — the index where the new product should be inserted.



## Constraints

- 1 ≤ n ≤ 10^5
- 1 ≤ product_id, target ≤ 10^9
- The IDs are sorted in non-decreasing order.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

binary-search, array, searching