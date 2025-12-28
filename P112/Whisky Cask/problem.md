## Title
Whisky Cask

## Slug
whisky-cask

## Difficulty
Easy

## Description
An investor buys a cask of scotch. They want to hold it while it ages and sell it to a bottler later.

You have a list of cask value for $n$ consecutive years. You want to make one perfect move: distill on one year and bottle on a different year in the future. You cannot bottle before you distill.

Your goal is to find the **maximum possible ROI** you can earn from this single transaction. If it is impossible to make any ROI (i.e., the cask value only goes down), you should return 0.

## Examples

### 1

#### Input
6
7 1 5 3 6 4

#### Output
5

#### Explanation
distill on year 2 (cask value = 1) and bottle on year 5 (cask value = 6). The ROI is $6 - 1 = 5$.
Note that distilling on year 1 (cask value = 7) is not optimal, as all future values are lower.

### 2

#### Input
5
7 6 4 3 1

#### Output
0

#### Explanation
The cask value never increases, so it is impossible to make a ROI. The maximum ROI is 0.

## Input Format
- The first line contains a single integer `n`, the number of years.
- The second line contains `n` space-separated integers representing the cask value on each year.

## Output Format
- Return a single integer representing the maximum ROI. If no ROI can be made, return 0.

## Constraints
- 1 ≤ n ≤ 10^5
- 0 ≤ values ≤ 10^4

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, dynamic-programming, greedy
