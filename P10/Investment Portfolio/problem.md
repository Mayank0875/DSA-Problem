## Title

Investment Portfolio

## Slug

investment-portfolio

## Difficulty

Medium

## Description

An investor has a portfolio of N assets, recorded chronologically. Each asset is classified as 'Risk' (0) or 'Growth' (1). A "balanced portfolio" must contain an equal number of Risk and Growth assets. The investor decides to sell off exactly one contiguous block of assets to rebalance. What is the minimum number of assets they must sell? If the portfolio is already balanced, they sell nothing (length 0).

## Examples

### 1

#### Input

6
[1, 0, 0, 0, 1, 0]

#### Output

2

#### Explanation

The portfolio has four 'Risk' (0) and two 'Growth' (1) assets. To balance, we must sell two more 0s than 1s.
The shortest segment that achieves this is [0, 0] at indices 2 and 3. 
The length of the removed segment is 2.


### 2

#### Input

6
[1, 1, 0, 0, 1, 0,]

#### Output

0

#### Explanation

The stream contains three 0s and three 1s. It is already balanced, so no segment needs to be removed. 
The length of the removed segment is 0.


## Input Format

- The first line contains a single integer N, the number of elements in the data stream.
- The second line contains N space-separated integers, where each integer is either 0 or 1.

## Output Format

- Return a single integer representing the length of the shortest contiguous segment that needs to be removed to balance the stream.

## Constraints

- 1 ≤ N ≤ 10^5
- 0 ≤ arr[i] ≤ 1

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

arrays, sliding window, prefix sum, hashmap