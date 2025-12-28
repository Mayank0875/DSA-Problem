## Title
Book Page Numbers

## Slug
book-page-numbers

## Difficulty
Medium

## Description
Pages in a book must be ordered. A binding error inserted a signature of pages upside down and backwards.

A valid book binding must be readable, meaning the page numbers should appear in non-decreasing order.

However, a binding error has inserted a chunk of incorrect page numbers into the middle of the book binding, corrupting it. To fix this, you must remove a single contiguous sequence of page numbers (a subarray) so that the remaining page numbers form a sorted, non-decreasing sequence.

Your goal is to minimize the pages removed. Determine the length of the **shortest contiguous subarray** that needs to be removed to restore the non-decreasing order of the remaining page numbers.

## Examples

### 1

#### Input
8
1 2 3 10 4 2 3 5

#### Output
3

#### Explanation
The shortest subarray to remove is `[10, 4, 2]` (indices 3, 4, 5). The remaining book binding is `[1, 2, 3, 3, 5]`, which is sorted. Removing `[3, 10, 4]` is also a valid solution of length 3.

### 2

#### Input
5
5 4 3 2 1

#### Output
4

#### Explanation
Since the book binding is strictly decreasing, we can only keep one page number. We must remove a subarray of length 4 (e.g., `[5, 4, 3, 2]` leaving `[1]`).

## Input Format
- The first line contains an integer `n`, the number of page numbers.
- The second line contains `n` space-separated integers representing the `pages` array.

## Output Format
- Return a single integer representing the length of the shortest subarray to remove.

## Constraints
- 1 ≤ n ≤ 10^5
- 0 ≤ pages[i] ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, two-pointers, binary-search
