## Title
Factory Defect Analysis

## Slug
factory-defect-analysis

## Difficulty
Medium

## Description
A quality control camera logs defects on an assembly line. A 'batch issue' is identified as a sequence of products exhibiting at most `k` distinct error codes.

The assembly line is represented as a sequence of products, where each product has a specific error code. You need to select a contiguous segment of the sequence.

However, there is a constraint: the segment is valid only if it contains **at most** `k` distinct error codes.

Given the sequence of products and the constraint `k`, your task is to calculate the total number of valid contiguous segments (subarrays).

## Examples

### 1

#### Input
5 2
1 2 3 1 1

#### Output
10

#### Explanation
The valid segments with at most 2 distinct values are:
[1], [2], [3], [1], [1] (length 1)
[1, 2], [2, 3], [3, 1], [1, 1] (length 2)
[3, 1, 1] (length 3)
Total = 10.

### 2

#### Input
5 1
1 2 3 4 5

#### Output
5

#### Explanation
Only single-element segments are valid because every pair has 2 distinct values, which exceeds k=1.

## Input Format
- The first line contains two integers `n` and `k`: the length of the sequence and the maximum allowed distinct values.
- The second line contains `n` integers representing the error codes of the products.

## Output Format
- Return one integer: the number of valid contiguous segments.

## Constraints
- 1 ≤ k ≤ n ≤ 2e5
- 1 ≤ value ≤ 2e5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
sliding-window, two-pointers, array
