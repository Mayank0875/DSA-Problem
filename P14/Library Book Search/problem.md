## Title

Library Book Search

## Slug

library-book-search

## Difficulty

Easy

## Description

A library's catalog is sorted by publication year. You are searching for all books from a specific `target` year. To see the next set of books, you need to find the index of the first book published in a year *strictly greater* than the `target` year. This helps you find the boundary between the two year groups.

You must write an algorithm with O(log n) runtime complexity.

## Examples

### 1

#### Input

6 8
[2, 5, 8, 8, 8, 12]


#### Output

5

#### Explanation

The books from year 8 are at indices 2, 3, and 4. The first book from a year strictly greater than 8 is from year 12, located at index 5.

### 2

#### Input

6 6
[2, 5, 7, 8, 11, 12]

#### Output

2

#### Explanation

There is no book from year 6. The first book from a year strictly greater than 6 is from year 7, which is at index 2.

## Input Format

- The first line contains an integers n and target , the number of grimoires and the ID of the grimoire to find. 
- The second line contains n space-separated integers representing the sorted grimoire IDs.


## Output Format

- Return a single integer representing the index of the first element strictly greater than the target.

## Constraints

- 1 ≤ n ≤ 10^5
- 1 ≤ grimoire_id, target ≤ 10^9
- The grimoire IDs are sorted in non-decreasing order.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

binary-search, array, searching