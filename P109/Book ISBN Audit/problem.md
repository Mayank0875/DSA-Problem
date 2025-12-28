## Title
Book ISBN Audit

## Slug
book-isbn-audit

## Difficulty
Easy

## Description
A bookstore imports a catalog. It checks for duplicate ISBNs to ensure database integrity.

Your task is to determine if any ISBN appears at least twice in the list.

## Examples

### 1

#### Input
4
1 2 3 1

#### Output
Yes

#### Explanation
The ISBN `1` appears twice.

### 2

#### Input
4
1 2 3 4

#### Output
No

#### Explanation
All ISBNs are distinct.

## Input Format
- The first line contains a single integer n, the number of books.
- The second line contains n space-separated integers, representing the ISBNs.

## Output Format
- Return `Yes` if any ISBN appears at least twice, otherwise `No`.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ values ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
sorting, array, hash-table
