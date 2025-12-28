## Title
Baseball Cards

## Slug
baseball-cards

## Difficulty
Easy

## Description
A kid tracks the value of a rookie card. They want to buy it and sell it after the player wins MVP.

You have a list of card value for $n$ consecutive seasons. You want to make one perfect move: collect on one season and trade on a different season in the future. You cannot trade before you collect.

Your goal is to find the **maximum possible increase** you can earn from this single transaction. If it is impossible to make any increase (i.e., the card value only goes down), you should return 0.

## Examples

### 1

#### Input
6
7 1 5 3 6 4

#### Output
5

#### Explanation
collect on season 2 (card value = 1) and trade on season 5 (card value = 6). The increase is $6 - 1 = 5$.
Note that collecting on season 1 (card value = 7) is not optimal, as all future values are lower.

### 2

#### Input
5
7 6 4 3 1

#### Output
0

#### Explanation
The card value never increases, so it is impossible to make a increase. The maximum increase is 0.

## Input Format
- The first line contains a single integer `n`, the number of seasons.
- The second line contains `n` space-separated integers representing the card value on each season.

## Output Format
- Return a single integer representing the maximum increase. If no increase can be made, return 0.

## Constraints
- 1 ≤ n ≤ 10^5
- 0 ≤ values ≤ 10^4

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, dynamic-programming, greedy
