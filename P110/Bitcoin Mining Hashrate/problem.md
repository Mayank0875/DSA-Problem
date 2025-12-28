## Title
Bitcoin Mining Hashrate

## Slug
bitcoin-mining-hashrate

## Difficulty
Easy

## Description
A miner overclocks their rig. A 'tuning ramp' is a sequence of tests where the hashrate strictly increases.

The Miner is analyzing a sequence of tests represented by an array of integers `nums`, where `nums[i]` represents the hashrate at index `i`.

The Miner wants to find the maximum total hashrate obtained during a single "**Tuning Ramp**". A "Tuning Ramp" is defined as a contiguous subarray of tests where the hashrate of each test is `strictly greater` than the previous one.

Your task is to find the **maximum sum** of hashrates possible from one such Tuning Ramp. The Tuning Ramp must include at least one test.

## Examples

### 1

#### Input
6
10 20 30 5 10 50

#### Output
65

#### Explanation
The The Miner identifies the sequence `[10, 20, 30]` with a sum of 60. However, a better Tuning Ramp starts later: `[5, 10, 50]`. This is a strictly increasing contiguous subarray, and its sum is 65.

### 2

#### Input
5
10 20 30 40 50

#### Output
150

#### Explanation
The entire sequence is strictly increasing. The sum is 150.

## Input Format
- The first line contains a single integer `n`, the number of tests.
- The second line contains `n` space-separated integers, representing the hashrates.

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
