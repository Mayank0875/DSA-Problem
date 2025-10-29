## Title

Distinct Books in Library Catalog

## Slug

distinct-books-library-catalog

## Difficulty

Easy

## Description

A librarian is reviewing the catalog entries for books recently added to the library. Each book is assigned an International Standard Book Number (ISBN), represented as a numerical code. Due to multiple copies or entry errors, the same ISBN might appear multiple times in the list. The librarian needs to find out how many unique book titles (represented by unique ISBNs) are in this recent batch. Given the list of ISBN codes, calculate the number of distinct books.

## Examples

### 1

#### Input

5
[2, 3, 2, 2, 3]

#### Output

2

#### Explanation

The ISBNs recorded are 2, 3, 2, 2, 3. The unique ISBNs are 2 and 3. There are 2 distinct book titles.

### 2

#### Input

8
[10, 5, 10, 2, 5, 10, 5, 2]

#### Output

3

#### Explanation

The unique ISBNs are 10, 5, and 2. There are 3 distinct book titles.

## Input Format

- The first line contains an integer n: the total number of catalog entries.
- The second line contains $n$ integers x_1, x_2, ...., x_n: the ISBN codes.

## Output Format

- Return a single integer: the count of distinct ISBN codes.

## Constraints

- 1 ≤ n ≤ 1e5
- 1 ≤ x_i ≤ 1e9

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

sorting, set, counting, library