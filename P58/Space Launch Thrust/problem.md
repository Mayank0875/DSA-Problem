## Title
Space Launch Thrust

## Slug
space-launch-thrust

## Difficulty
Medium

## Description
A rocket uses two boosters. Their combined thrust must equal the escape velocity requirement for the payload. Given available boosters, count the valid launch configurations.

## Examples

### 1

#### Input
6 6
1 5 7 -1 5 1

#### Output
6

#### Explanation
Pairs with sum 6:
(1, 5), (1, 5), (5, 1), (5, 1), (7, -1), (1, 5)...
Total valid pairs count is 6.

### 2

#### Input
4 2
1 1 1 1

#### Output
6

#### Explanation
Every combination of two '1's sums to 2. The number of ways to choose 2 items from 4 is 6.

## Input Format
- The first line contains an integer n and `target`, the number of elements and the target sum.
- The second line contains n space-separated integers representing the array.

## Output Format
- Return a single integer — total number of valid pairs.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ target ≤ 10^9
- -10^9 ≤ arr[i] ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, hash-table
