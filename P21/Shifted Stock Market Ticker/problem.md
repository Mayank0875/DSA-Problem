## Title

Shifted Stock Market Ticker

## Slug

shifted-stock-market-ticker

## Difficulty

Medium

## Description

A list of stock prices (as unique integers) for a day was sorted from low to high. A data feed error "rotated" this list, starting it from an arbitrary point (e.g., [10, 20, 30] became [20, 30, 10]). To analyze the day's trading, you need to find the lowest price of the day (the minimum value) from this rotated list. Your algorithm must run in O(log n) time.

## Examples

### 1

#### Input

7
[4, 5, 6, 7, 0, 1, 2]

#### Output

0

#### Explanation

The smallest value in this rotated sequence is 0.

### 2

#### Input

6
[4, 5, 6, 7, 1, 2]

#### Output

1

#### Explanation

The smallest value in this rotated sequence is 1.

## Input Format

- The first line contains an integer n, the number of items.
- The second line contains n space-separated integers representing the item numbers after rotation. All numbers are unique.

## Output Format

- Return a single integer representing the minimum item number found.

## Constraints

- 1 ≤ n ≤ 10^5
- 1 ≤ gem_number ≤ 10^9
- The array is guaranteed to be a rotation of a sorted array.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

binary-search, array