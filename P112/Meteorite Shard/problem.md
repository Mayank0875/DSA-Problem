## Title
Meteorite Shard

## Slug
meteorite-shard

## Difficulty
Easy

## Description
A hunter tracks the price per gram of moon rocks. They want to buy a shard and sell it to a museum.

You have a list of price per gram for $n$ consecutive weeks. You want to make one perfect move: find on one week and deal on a different week in the future. You cannot deal before you find.

Your goal is to find the **maximum possible cash** you can earn from this single transaction. If it is impossible to make any cash (i.e., the price per gram only goes down), you should return 0.

## Examples

### 1

#### Input
6
7 1 5 3 6 4

#### Output
5

#### Explanation
find on week 2 (price per gram = 1) and deal on week 5 (price per gram = 6). The cash is $6 - 1 = 5$.
Note that finding on week 1 (price per gram = 7) is not optimal, as all future values are lower.

### 2

#### Input
5
7 6 4 3 1

#### Output
0

#### Explanation
The price per gram never increases, so it is impossible to make a cash. The maximum cash is 0.

## Input Format
- The first line contains a single integer `n`, the number of weeks.
- The second line contains `n` space-separated integers representing the price per gram on each week.

## Output Format
- Return a single integer representing the maximum cash. If no cash can be made, return 0.

## Constraints
- 1 ≤ n ≤ 10^5
- 0 ≤ values ≤ 10^4

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, dynamic-programming, greedy
