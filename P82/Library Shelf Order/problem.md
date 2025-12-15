## Title
Library Shelf Order

## Slug
library-shelf-order

## Difficulty
Easy

## Description
A librarian checks n books on a shelf. They want to find the longest subsequence that is already in correct ascending Dewey Decimal order.

You have Dewey numbers for n books.
A sorted sequence consists of books where the number is strictly higher than the previous book.

You must check the shelf to find the longest possible sorted sequence. You can skip any number of books to form the sequence, but you must maintain the original shelf order order of the selected books. Calculate the maximum number of books that can form such a sequence.

## Examples

### 1

#### Input
8
7 3 5 3 6 2 9 8

#### Output
4

#### Explanation
The input contains: [7, 3, 5, 3, 6, 2, 9, 8]. The longest sorted sequences (strictly increasing) include:
3, 5, 6, 9
3, 5, 6, 8
The length of these sequences is 4.

### 2

#### Input
5
5 4 3 2 1

#### Output
1

#### Explanation
Since the values are strictly decreasing, we can pick at most 1 book.

## Input Format
- The first line contains an integer n: the number of books.
- The second line contains n integers x_1, x_2 ... x_n: the Dewey number of each book in order.

## Output Format
- Return one integer: the length of the longest valid sorted sequence.

## Constraints
- 1 ≤ n ≤ 2e5
- 1 ≤ x ≤ 1e9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
binary-search, dynamic-programming, greedy
