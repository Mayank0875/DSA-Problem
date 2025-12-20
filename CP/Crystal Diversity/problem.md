## Title

Crystal Diversity

## Slug

crystal-diversity

## Difficulty

Medium

## Description

A geologist is exploring a newly discovered crystal vein. The vein is represented as a sequence of minerals, where each mineral has a specific type ID. The geologist wants to extract a contiguous segment of the vein for analysis.

However, the analysis equipment has a limitation: it can process a segment only if it contains at most $k$ distinct types of minerals.

Given the sequence of mineral types and the equipment's constraint $k$, your task is to calculate the total number of contiguous segments (subarrays) that satisfy this condition.

## Examples

### 1

#### Input

5 2
1 2 3 1 1

#### Output

10

#### Explanation

The valid subarrays with at most 2 distinct values are:
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

Only single-element subarrays are valid because every pair has 2 distinct values, which exceeds $k=1$.
  

## Input Format  

- The first line contains two integers $n$ and $k$: the length of the array and the maximum allowed distinct values.
- The second line contains $n$ integers x_1, x_2, ...., x_n: the types of minerals.

## Output Format  

- Return one integer: the number of valid subarrays.
  

## Constraints  

- 1 ≤ k ≤ n ≤ 2e5
- 1 ≤ x_i ≤ 2e5

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

sliding-window, two-pointers, sorting, array