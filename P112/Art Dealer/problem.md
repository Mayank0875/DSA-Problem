## Title
Art Dealer

## Slug
art-dealer

## Difficulty
Easy

## Description
You are watching the estimated value of a Banksy piece. You want to buy it at an auction and sell it to a gallery later.

You have a list of appraisal value for $n$ consecutive months. You want to make one perfect move: bid on one month and consign on a different month in the future. You cannot consign before you bid.

Your goal is to find the **maximum possible commission** you can earn from this single transaction. If it is impossible to make any commission (i.e., the appraisal value only goes down), you should return 0.

## Examples

### 1

#### Input
6
7 1 5 3 6 4

#### Output
5

#### Explanation
bid on month 2 (appraisal value = 1) and consign on month 5 (appraisal value = 6). The commission is $6 - 1 = 5$.
Note that biding on month 1 (appraisal value = 7) is not optimal, as all future values are lower.

### 2

#### Input
5
7 6 4 3 1

#### Output
0

#### Explanation
The appraisal value never increases, so it is impossible to make a commission. The maximum commission is 0.

## Input Format
- The first line contains a single integer `n`, the number of months.
- The second line contains `n` space-separated integers representing the appraisal value on each month.

## Output Format
- Return a single integer representing the maximum commission. If no commission can be made, return 0.

## Constraints
- 1 ≤ n ≤ 10^5
- 0 ≤ values ≤ 10^4

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, dynamic-programming, greedy
