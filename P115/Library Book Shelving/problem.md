## Title
Library Book Shelving

## Slug
library-book-shelving

## Difficulty
Medium

## Description
A librarian finds a shelf of books where the call numbers are mostly sorted, but a block of books was shoved in randomly.

A valid shelf must be organized, meaning the call numbers should appear in non-decreasing order.

However, a careless patron has inserted a chunk of incorrect call numbers into the middle of the shelf, corrupting it. To fix this, you must remove a single contiguous sequence of call numbers (a subarray) so that the remaining call numbers form a sorted, non-decreasing sequence.

Your goal is to minimize the number of unshelved books. Determine the length of the **shortest contiguous subarray** that needs to be removed to restore the non-decreasing order of the remaining call numbers.

## Examples

### 1

#### Input
8
1 2 3 10 4 2 3 5

#### Output
3

#### Explanation
The shortest subarray to remove is `[10, 4, 2]` (indices 3, 4, 5). The remaining shelf is `[1, 2, 3, 3, 5]`, which is sorted. Removing `[3, 10, 4]` is also a valid solution of length 3.

### 2

#### Input
5
5 4 3 2 1

#### Output
4

#### Explanation
Since the shelf is strictly decreasing, we can only keep one call number. We must remove a subarray of length 4 (e.g., `[5, 4, 3, 2]` leaving `[1]`).

## Input Format
- The first line contains an integer `n`, the number of call numbers.
- The second line contains `n` space-separated integers representing the `books` array.

## Output Format
- Return a single integer representing the length of the shortest subarray to remove.

## Constraints
- 1 ≤ n ≤ 10^5
- 0 ≤ books[i] ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, two-pointers, binary-search
