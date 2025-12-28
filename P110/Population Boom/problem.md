## Title
Population Boom

## Slug
population-boom

## Difficulty
Easy

## Description
A demographer looks at census data. A 'Boom Era' is a series of years where the population count strictly increased.

The Researcher is analyzing a sequence of years represented by an array of integers `nums`, where `nums[i]` represents the population count at index `i`.

The Researcher wants to find the maximum total population count obtained during a single "**Boom Era**". A "Boom Era" is defined as a contiguous subarray of years where the population count of each year is `strictly greater` than the previous one.

Your task is to find the **maximum sum** of population counts possible from one such Boom Era. The Boom Era must include at least one year.

## Examples

### 1

#### Input
6
10 20 30 5 10 50

#### Output
65

#### Explanation
The The Researcher identifies the sequence `[10, 20, 30]` with a sum of 60. However, a better Boom Era starts later: `[5, 10, 50]`. This is a strictly increasing contiguous subarray, and its sum is 65.

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
- The second line contains `n` space-separated integers, representing the population counts.

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
