## Title
Book Chapter Navigation

## Slug
book-chapter-navigation

## Difficulty
Easy

## Description
An e-reader app stores the starting page numbers of all chapters in a sorted array. A user jumps to a specific page. The app needs to figure out which chapter or section follows that page. Find the index of the first chapter start page that is greater than or equal to the user's current page.
The data is sorted in non-decreasing order.
You must write an algorithm with O(log n) runtime complexity.

## Examples

### 1

#### Input
6 8
2 5 7 8 11 12

#### Output
3

#### Explanation
The first element greater than or equal to 8 is 8, which is at index 3.

### 2

#### Input
6 6
2 5 7 8 11 12

#### Output
2

#### Explanation
There is no element 6. The first element greater than 6 is 7, which is at index 2.

## Input Format
- The first line contains two integers n and target, the number of elements and the value to search/insert.
- The second line contains n space-separated integers representing the sorted sequence.

## Output Format
- Return a single integer representing the index (0-based) of the first element that is greater than or equal to the target. If all elements are smaller, return n.

## Constraints
- 1 ≤ n ≤ 10^5
- 1 ≤ value, target ≤ 10^9
- The sequence is sorted in non-decreasing order.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
binary-search, array, searching
