## Title
Last Lower Gold Price

## Slug
last-lower-gold-price

## Difficulty
Easy

## Description
You are a commodities trader analyzing the hourly price of gold. You have a sequence of price points. To identify short-term support levels, you want to find the price at the nearest previous hour that was strictly lower than the current hour's price. This information is critical for algorithmic trading bots to make buy/sell decisions based on recent trends. For each price point in the sequence, you need to find the value of the most recent preceding price that was strictly lower. If no such price exists because the market has been falling or flat, you should report this. Your task is to analyze the gold price sequence.

## Examples

### 1

#### Input
8
[100, 80, 60, 70, 60, 75, 85, 110]

#### Output
[-1, -1, -1, 60, -1, 60, 75, 85]

#### Explanation
Index 0 (100): No previous value, output -1.
Index 1 (80): 100 is not lower, output -1.
Index 2 (60): 100, 80 are not lower, output -1.
Index 3 (70): 60 is the nearest lower value, output 60.
Index 4 (60): No strictly lower previous value, output -1.
Index 5 (75): 60 at index 4 is nearest lower, output 60.
Index 6 (85): 75 at index 5 is nearest lower, output 75.
Index 7 (110): 85 at index 6 is nearest lower, output 85.

### 2

#### Input
5
50 50 50 50 50

#### Output
[-1, -1, -1, -1, -1]

#### Explanation
All values are equal, so no strictly lower previous value exists for any element.

## Input Format
The first line contains a single integer n, the number of elements.
The second line contains n space-separated integers representing the data sequence.

## Output Format
Return array of integers. The i-th integer should be the value of the nearest element j < i such that val_j < val_i. If no such element exists, return -1.

## Constraints
1 ≤ n ≤ 10^5
1 ≤ val_i ≤ 10^9 for all 0 ≤ i < n.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
stack, array
