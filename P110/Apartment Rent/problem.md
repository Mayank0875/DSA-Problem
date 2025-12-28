## Title
Apartment Rent

## Slug
apartment-rent

## Difficulty
Easy

## Description
A tenant looks at rent history. A 'Market Hike' is a sequence of years where the rent strictly increased.

The Tenant is analyzing a sequence of years represented by an array of integers `nums`, where `nums[i]` represents the rent cost at index `i`.

The Tenant wants to find the maximum total rent cost obtained during a single "**Market Hike**". A "Market Hike" is defined as a contiguous subarray of years where the rent cost of each year is `strictly greater` than the previous one.

Your task is to find the **maximum sum** of rent costs possible from one such Market Hike. The Market Hike must include at least one year.

## Examples

### 1

#### Input
6
10 20 30 5 10 50

#### Output
65

#### Explanation
The The Tenant identifies the sequence `[10, 20, 30]` with a sum of 60. However, a better Market Hike starts later: `[5, 10, 50]`. This is a strictly increasing contiguous subarray, and its sum is 65.

### 2

#### Input
5
10 20 30 40 50

#### Output
150

#### Explanation
The entire sequence is strictly increasing. The sum is 150.

## Input Format
- The first line contains a single integer `n`, the number of years.
- The second line contains `n` space-separated integers, representing the rent costs.

## Output Format
- Return a single integer representing the maximum sum of any strictly increasing contiguous subarray.

## Constraints
- 1 ≤ n ≤ 100
- 1 ≤ nums[i] ≤ 100

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, sliding-window, easy
