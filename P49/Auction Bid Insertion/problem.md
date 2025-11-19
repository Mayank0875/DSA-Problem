## Title
Auction Bid Insertion

## Slug
auction-bid-insertion

## Difficulty
Easy

## Description
An online auction system maintains a list of current bids sorted from lowest to highest. A new bid has just been placed. To update the display efficiently, the system needs to know the correct index where this new bid should be inserted to keep the list sorted. If there are existing bids equal to the new one, the new bid should be placed before them (conceptually, or simply find the first index >= new bid).
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
