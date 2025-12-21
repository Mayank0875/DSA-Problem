## Title
Stock Market Ticker

## Slug
stock-market-ticker

## Difficulty
Medium

## Description
A trader groups ticks into candles. Each tick has a price change.

The Trader is working with a sequence of $n$ ticks, where the $i$-th tick has a value of $a_i$.

The Trader needs to create a **chart pattern**. A chart pattern involves dividing the sequence of $n$ ticks into one or more contiguous candles such that every tick belongs to exactly one candle.

For a specific chart pattern, the **volatility index** is calculated as follows:
1. Calculate the sum of values for each candle in the partition.
2. The volatility index is the bitwise XOR sum of these candle sums.

Your task is to calculate the bitwise XOR sum of the volatility index values of **all possible chart patterns** of the sequence.

## Examples

### 1

#### Input
1
1

#### Output
1

#### Explanation
Total XOR sum: 1.

### 2

#### Input
2
1 2

#### Output
0

#### Explanation
Partition {1}, {2}: Group sums are 1, 2. XOR sum = 1 ^ 2 = 3.
Partition {1, 2}: Group sum is 3. XOR sum = 3.
Total Result = 3 ^ 3 = 0.

## Input Format
- The first line contains a single integer $n$ — the length of the sequence.
- The second line contains $n$ space-separated integers $a_1, a_2, \dots, a_n$.

## Output Format
- Return a single integer representing the total XOR sum of volatility indexs of all possible partitions.

## Constraints
- 1 ≤ n ≤ 10^6
- 1 ≤ a_i ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths, dynamic-programming, array
