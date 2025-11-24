## Title
Fabric Cutting Waste

## Slug
fabric-cutting-waste

## Difficulty
Medium

## Description
A tailor cuts fabric from rolls. They have scraps of various lengths. They want to sew two scraps together to form a piece of a specific required length. Count the number of scrap pairs that can be used.

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
