## Title
Real Estate Mogul

## Slug
real-estate-mogul

## Difficulty
Easy

## Description
You are looking at property value trends in a developing neighborhood. You want to buy a plot of land and sell it later for the biggest margin.

You have a list of property price for $n$ consecutive years. You want to make one perfect move: invest on one year and divest on a different year in the future. You cannot divest before you invest.

Your goal is to find the **maximum possible margin** you can earn from this single transaction. If it is impossible to make any margin (i.e., the property price only goes down), you should return 0.

## Examples

### 1

#### Input
6
7 1 5 3 6 4

#### Output
5

#### Explanation
invest on year 2 (property price = 1) and divest on year 5 (property price = 6). The margin is $6 - 1 = 5$.
Note that investing on year 1 (property price = 7) is not optimal, as all future values are lower.

### 2

#### Input
5
7 6 4 3 1

#### Output
0

#### Explanation
The property price never increases, so it is impossible to make a margin. The maximum margin is 0.

## Input Format
- The first line contains a single integer `n`, the number of years.
- The second line contains `n` space-separated integers representing the property price on each year.

## Output Format
- Return a single integer representing the maximum margin. If no margin can be made, return 0.

## Constraints
- 1 ≤ n ≤ 10^5
- 0 ≤ values ≤ 10^4

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, dynamic-programming, greedy
