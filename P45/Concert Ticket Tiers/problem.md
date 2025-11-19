## Title
Concert Ticket Tiers

## Slug
concert-ticket-tiers

## Difficulty
Medium

## Description
Tickets for a concert are sold at different price points (tiers). The sales ledger lists the price of every ticket sold, sorted by amount. The promoter wants to count how many tickets were sold for a specific price tier.
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
