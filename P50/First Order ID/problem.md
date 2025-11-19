## Title
First Order ID

## Slug
first-order-id

## Difficulty
Easy

## Description
An order processing system lists Order IDs sorted numerically. A support rep needs to locate the first entry of a specific Order ID to check its status. Given the sorted list of Order IDs, find the index of the first occurrence of the target ID.
The data is sorted in non-decreasing order.
You must write an algorithm with O(log n) runtime complexity.

## Examples

### 1

#### Input
6 8
2 8 8 8 9 9

#### Output
1

#### Explanation
The target value 8 first appears at index 1.

### 2

#### Input
6 6
2 5 7 8 11 12

#### Output
-1

#### Explanation
The target value 6 is not found in the list.

## Input Format
- The first line contains two integers n and target, the number of elements and the value to find.
- The second line contains n space-separated integers representing the sorted sequence.

## Output Format
- Return a single integer: the index of the first occurrence of the target, or -1 if it is not found.

## Constraints
- 1 ≤ n ≤ 10^5
- 1 ≤ value, target ≤ 10^9
- The sequence is sorted in non-decreasing order.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
binary-search, array, searching, first-occurrence
