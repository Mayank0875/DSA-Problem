## Title
Library Book Loans

## Slug
library-book-loans

## Difficulty
Easy

## Description
A librarian tracks daily loans. A 'Summer Reading Craze' is a week where daily loans strictly increase.

The Librarian is analyzing a sequence of days represented by an array of integers `nums`, where `nums[i]` represents the loan count at index `i`.

The Librarian wants to find the maximum total loan count obtained during a single "**Summer Reading Craze**". A "Summer Reading Craze" is defined as a contiguous subarray of days where the loan count of each day is `strictly greater` than the previous one.

Your task is to find the **maximum sum** of loan counts possible from one such Summer Reading Craze. The Summer Reading Craze must include at least one day.

## Examples

### 1

#### Input
6
10 20 30 5 10 50

#### Output
65

#### Explanation
The The Librarian identifies the sequence `[10, 20, 30]` with a sum of 60. However, a better Summer Reading Craze starts later: `[5, 10, 50]`. This is a strictly increasing contiguous subarray, and its sum is 65.

### 2

#### Input
5
10 20 30 40 50

#### Output
150

#### Explanation
The entire sequence is strictly increasing. The sum is 150.

## Input Format
- The first line contains a single integer `n`, the number of days.
- The second line contains `n` space-separated integers, representing the loan counts.

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
