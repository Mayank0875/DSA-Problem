## Title
Baking Temperature

## Slug
baking-temperature

## Difficulty
Easy

## Description
A baker monitors an oven. A 'Preheat Surge' is a sequence of readings where the temperature strictly rises.

The Baker is analyzing a sequence of readings represented by an array of integers `nums`, where `nums[i]` represents the degree at index `i`.

The Baker wants to find the maximum total degree obtained during a single "**Preheat Surge**". A "Preheat Surge" is defined as a contiguous subarray of readings where the degree of each reading is `strictly greater` than the previous one.

Your task is to find the **maximum sum** of degrees possible from one such Preheat Surge. The Preheat Surge must include at least one reading.

## Examples

### 1

#### Input
6
10 20 30 5 10 50

#### Output
65

#### Explanation
The The Baker identifies the sequence `[10, 20, 30]` with a sum of 60. However, a better Preheat Surge starts later: `[5, 10, 50]`. This is a strictly increasing contiguous subarray, and its sum is 65.

### 2

#### Input
5
10 20 30 40 50

#### Output
150

#### Explanation
The entire sequence is strictly increasing. The sum is 150.

## Input Format
- The first line contains a single integer `n`, the number of readings.
- The second line contains `n` space-separated integers, representing the degrees.

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
