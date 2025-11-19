## Title
First Available Seat

## Slug
first-available-seat

## Difficulty
Easy

## Description
A theater booking system lists occupied seat numbers in sorted order. For a debugging task, the admin needs to find the first entry in the database for a specific seat number (to check for duplicate booking errors). Given the sorted list of booked seat numbers, return the index of the first occurrence of the target seat number.
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
