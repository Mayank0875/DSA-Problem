## Title
Foreign Exchange

## Slug
foreign-exchange

## Difficulty
Easy

## Description
A traveler watches the exchange rate between USD and EUR. They want to convert their cash once to get the most Euros later.

You have a list of exchange rate for $n$ consecutive days. You want to make one perfect move: convert on one day and exchange back on a different day in the future. You cannot exchange back before you convert.

Your goal is to find the **maximum possible yield** you can earn from this single transaction. If it is impossible to make any yield (i.e., the exchange rate only goes down), you should return 0.

## Examples

### 1

#### Input
6
7 1 5 3 6 4

#### Output
5

#### Explanation
convert on day 2 (exchange rate = 1) and exchange back on day 5 (exchange rate = 6). The yield is $6 - 1 = 5$.
Note that converting on day 1 (exchange rate = 7) is not optimal, as all future values are lower.

### 2

#### Input
5
7 6 4 3 1

#### Output
0

#### Explanation
The exchange rate never increases, so it is impossible to make a yield. The maximum yield is 0.

## Input Format
- The first line contains a single integer `n`, the number of days.
- The second line contains `n` space-separated integers representing the exchange rate on each day.

## Output Format
- Return a single integer representing the maximum yield. If no yield can be made, return 0.

## Constraints
- 1 ≤ n ≤ 10^5
- 0 ≤ values ≤ 10^4

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, dynamic-programming, greedy
