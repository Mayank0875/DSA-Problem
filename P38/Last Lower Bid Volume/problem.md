## Title
Last Lower Bid Volume

## Slug
last-lower-bid-volume

## Difficulty
Easy

## Description
You are a financial analyst looking at the volume of bids in a stock order book over time. You have a list of bid volumes. To detect sudden increases in market interest, you want to find the volume of the nearest previous entry that was strictly lower than the current volume. This helps in flagging momentum shifts. For each volume entry, you need to determine the value of the most recent prior entry that was strictly smaller. If all previous volumes were higher or equal, you should report this result. Your task is to calculate this metric for the order book history.

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
