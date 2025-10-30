## Title

Gene Expression Peak

## Slug

gene-expression-peak

## Difficulty

Medium

## Description

You are studying a DNA strand with N genes, whose expression levels are in array A. You are analyzing segments of K consecutive genes. For each segment (window) of size K, find the gene with the *highest expression level* (MAX value). To get a final checksum for your research, calculate the XOR of all these maximum expression levels.

## Examples

### 1

#### Input

5 3
[1, 2, 3, 4, 5]

#### Output

2

#### Explanation

All windows of size 3 are:
    •   [1, 2, 3] → MAX = 3
    •   [2, 3, 4] → MAX = 4
    •   [3, 4, 5] → MAX = 5

Final XOR = 3 ^ 4 ^ 5 = 2

### 2

#### Input

4 2
[5, 1, 3, 2]

#### Output

5

#### Explanation

Windows:
    •   [5, 1] → MAX = 5
    •   [1, 3] → MAX = 3
    •   [3, 2] → MAX = 3

Final XOR = 5 ^ 3 ^ 3 = 5

## Input Format

- The first line contains two integers N (size of array) and K (window size).
- The second line contains N space-separated integers — the elements of the array.

## Output Format

- Return a single integer — the final XOR of all window XORs.

## Constraints

- 1 ≤ N ≤ 10^5
- 1 ≤ K ≤ N
- 0 ≤ arr[i] ≤ 1e9

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

arrays, sliding window, deque