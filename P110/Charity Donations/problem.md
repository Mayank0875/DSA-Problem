## Title
Charity Donations

## Slug
charity-donations

## Difficulty
Easy

## Description
A charity tracks hourly donations during a telethon. A 'Giving Momentum' streak occurs when hourly totals strictly rise.

The Organizer is analyzing a sequence of hours represented by an array of integers `nums`, where `nums[i]` represents the donation total at index `i`.

The Organizer wants to find the maximum total donation total obtained during a single "**Giving Momentum**". A "Giving Momentum" is defined as a contiguous subarray of hours where the donation total of each hour is `strictly greater` than the previous one.

Your task is to find the **maximum sum** of donation totals possible from one such Giving Momentum. The Giving Momentum must include at least one hour.

## Examples

### 1

#### Input
6
10 20 30 5 10 50

#### Output
65

#### Explanation
The The Organizer identifies the sequence `[10, 20, 30]` with a sum of 60. However, a better Giving Momentum starts later: `[5, 10, 50]`. This is a strictly increasing contiguous subarray, and its sum is 65.

### 2

#### Input
5
10 20 30 40 50

#### Output
150

#### Explanation
The entire sequence is strictly increasing. The sum is 150.

## Input Format
- The first line contains a single integer `n`, the number of hours.
- The second line contains `n` space-separated integers, representing the donation totals.

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
