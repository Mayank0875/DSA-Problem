## Title

Stock Trend XOR Indicator

## Slug

stock-trend-xor-indicator

## Difficulty

Easy

## Description

An analyst is studying a sequence of daily stock price changes A₁, A₂, ..., Aₙ (represented as integers). To identify short-term volatility patterns, they use a sliding window of size K. For each K-day period (window), they calculate an indicator value by XORing the price changes within that window. To get a single metric summarizing the volatility across the entire period, they XOR together all the calculated indicator values. Compute this final volatility metric.

## Examples

### 1

#### Input

5 3
[1, 2, 3, 4, 5]

#### Output

7

#### Explanation

Price change windows of size 3:
    •   [1, 2, 3] → Indicator (XOR) = 0
    •   [2, 3, 4] → Indicator (XOR) = 5
    •   [3, 4, 5] → Indicator (XOR) = 2

Final Volatility Metric = 0 ^ 5 ^ 2 = 7

### 2

#### Input

4 2
[5, 1, 3, 2]

#### Output

7

#### Explanation

Windows:
    •   [5, 1] → XOR = 4
    •   [1, 3] → XOR = 2
    •   [3, 2] → XOR = 1

Final Volatility Metric = 4 ^ 2 ^ 1 = 7

## Input Format

- The first line contains two integers N (number of days) and K (window size).
- The second line contains N space-separated integers — the daily price changes.

## Output Format

- Return a single integer — the final volatility metric.

## Constraints

- 1 ≤ N ≤ 10^5
- 1 ≤ K ≤ N
- 0 ≤ arr[i] ≤ 1e9 (Price changes can be non-negative for simplicity, or adjust range if needed)

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

arrays, sliding window, finance, bit manipulation