## Title

Packing Books onto Shelves

## Slug

packing-books-shelves

## Difficulty

Easy

## Description

A librarian is organizing books onto shelves. Each shelf section can hold one or two books side-by-side. The total width of the book(s) in one section cannot exceed the section width `x`. Given the widths of `n` books, determine the minimum number of shelf sections needed to accommodate all the books, respecting the width constraint.

## Examples

### 1

#### Input

4 10
[7, 2, 3, 9]

#### Output

3

#### Explanation

One efficient arrangement:
    - Section 1: Book of width 2 and book of width 7 (Total width 9 <= 10)
    - Section 2: Book of width 3 (Total width 3 <= 10)
    - Section 3: Book of width 9 (Total width 9 <= 10)
This requires 3 sections.

### 2

#### Input

5 5
[2, 2, 2, 3, 4]

#### Output

3

#### Explanation

One efficient arrangement:
    - Section 1: Book of width 2 and book of width 3 (Total width 5 <= 5)
    - Section 2: Two books of width 2 (Total width 4 <= 5)
    - Section 3: Book of width 4 (Total width 4 <= 5)
This requires 3 sections.

## Input Format

- The first line contains two integers n and x: the number of books and the maximum width per shelf section.
- The second line contains n integers p_1, p_2, ..., p_n: the width of each book.

## Output Format

- Return a single integer: the minimum number of shelf sections required.

## Constraints

- 1 ≤ n ≤ 1e5
- 1 ≤ x ≤ 1e9
- 1 ≤ p_i ≤ x

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

greedy, sorting, two pointers