## Title

Farmer's Maximum Yield

## Slug

farmers-maximum-yield

## Difficulty

Medium

## Description

A farmer has a long field divided into $N$ plots, arranged in a single line. They have recorded the net yield for each plot in a sequence. A positive number means a profit from that plot, while a negative number means a loss (due to pests or bad soil). The farmer wants to find the most profitable continuous segment of their field to focus on next season.

Your task is to find the contiguous subarray (containing at least one plot) that has the largest possible sum of yields.

## Examples

### 1

#### Input

9 
[-2, 1, -3, 4, -1, 2, 1, -5, 4]

#### Output

6

#### Explanation

The contiguous subarray (plots) `[4, -1, 2, 1]` has the largest sum of 6.
    
### 2

#### Input

1
[1]

#### Output

1

#### Explanation

The subarray `[1]` is the only option and has a sum of 1.
  

## Input Format  

- The first line contains a single integer $N$, the number of plots.
- The second line contains N space-separated integers, yield_i, representing the yield of each plot.

## Output Format  

- Return single integer representing the maximum sum of any contiguous subarray.
  

## Constraints  

- 1 ≤ n ≤ 1e5
- -1e4 ≤ yeild[i] ≤ 1e4

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

array, dynamic-programming, greedy