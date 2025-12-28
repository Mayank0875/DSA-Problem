## Title
Vintage Wine

## Slug
vintage-wine

## Difficulty
Easy

## Description
A sommelier tracks the price of a 1945 Romanée-Conti. They want to buy a bottle and sell it at the peak of its maturity curve.

You have a list of bottle price for $n$ consecutive years. You want to make one perfect move: cellar on one year and auction on a different year in the future. You cannot auction before you cellar.

Your goal is to find the **maximum possible appreciation** you can earn from this single transaction. If it is impossible to make any appreciation (i.e., the bottle price only goes down), you should return 0.

## Examples

### 1

#### Input
6
7 1 5 3 6 4

#### Output
5

#### Explanation
cellar on year 2 (bottle price = 1) and auction on year 5 (bottle price = 6). The appreciation is $6 - 1 = 5$.
Note that cellaring on year 1 (bottle price = 7) is not optimal, as all future values are lower.

### 2

#### Input
5
7 6 4 3 1

#### Output
0

#### Explanation
The bottle price never increases, so it is impossible to make a appreciation. The maximum appreciation is 0.

## Input Format
- The first line contains a single integer `n`, the number of years.
- The second line contains `n` space-separated integers representing the bottle price on each year.

## Output Format
- Return a single integer representing the maximum appreciation. If no appreciation can be made, return 0.

## Constraints
- 1 ≤ n ≤ 10^5
- 0 ≤ values ≤ 10^4

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, dynamic-programming, greedy
