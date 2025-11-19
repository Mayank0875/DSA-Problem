## Title
Shoe Inventory Tracker

## Slug
shoe-inventory-tracker

## Difficulty
Medium

## Description
A shoe store manager organizes inventory by size on a long shelf. The boxes are arranged in increasing order of shoe size. A customer asks how many pairs of a specific size are available. You need to efficiently determine the exact count of that specific size.
The data is sorted in non-decreasing order.
You must write an algorithm with O(log n) runtime complexity.

## Examples

### 1

#### Input
6 8
2 8 8 8 11 12

#### Output
3

#### Explanation
The target value 8 appears 3 times in the sorted list.

### 2

#### Input
6 6
2 5 7 8 11 12

#### Output
0

#### Explanation
The target value 6 appears 0 times in the sorted list.

## Input Format
- The first line contains two integers n and target, the number of items and the specific value to count.
- The second line contains n space-separated integers representing the sorted data sequence.

## Output Format
- Return a single integer representing the total number of times the target appears.

## Constraints
- 1 ≤ n ≤ 10^5
- 1 ≤ value, target ≤ 10^9
- The sequence is sorted in non-decreasing order.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
binary-search, array
