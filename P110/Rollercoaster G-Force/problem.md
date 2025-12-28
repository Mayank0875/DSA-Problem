## Title
Rollercoaster G-Force

## Slug
rollercoaster-g-force

## Difficulty
Easy

## Description
An engineer tests a ride. An 'Intensifying Loop' is a section of track where the G-force readings strictly increase every second.

The Engineer is analyzing a sequence of readings represented by an array of integers `nums`, where `nums[i]` represents the G-force unit at index `i`.

The Engineer wants to find the maximum total G-force unit obtained during a single "**Intensifying Loop**". A "Intensifying Loop" is defined as a contiguous subarray of readings where the G-force unit of each reading is `strictly greater` than the previous one.

Your task is to find the **maximum sum** of G-force units possible from one such Intensifying Loop. The Intensifying Loop must include at least one reading.

## Examples

### 1

#### Input
6
10 20 30 5 10 50

#### Output
65

#### Explanation
The The Engineer identifies the sequence `[10, 20, 30]` with a sum of 60. However, a better Intensifying Loop starts later: `[5, 10, 50]`. This is a strictly increasing contiguous subarray, and its sum is 65.

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
- The second line contains `n` space-separated integers, representing the G-force units.

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
