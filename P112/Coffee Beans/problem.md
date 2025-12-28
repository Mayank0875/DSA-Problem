## Title
Coffee Beans

## Slug
coffee-beans

## Difficulty
Easy

## Description
A roaster tracks the price of Arabica beans. They want to buy a shipment and sell it to cafes when supply is low.

You have a list of bean price for $n$ consecutive days. You want to make one perfect move: import on one day and distribute on a different day in the future. You cannot distribute before you import.

Your goal is to find the **maximum possible margin** you can earn from this single transaction. If it is impossible to make any margin (i.e., the bean price only goes down), you should return 0.

## Examples

### 1

#### Input
6
7 1 5 3 6 4

#### Output
5

#### Explanation
import on day 2 (bean price = 1) and distribute on day 5 (bean price = 6). The margin is $6 - 1 = 5$.
Note that importing on day 1 (bean price = 7) is not optimal, as all future values are lower.

### 2

#### Input
5
7 6 4 3 1

#### Output
0

#### Explanation
The bean price never increases, so it is impossible to make a margin. The maximum margin is 0.

## Input Format
- The first line contains a single integer `n`, the number of days.
- The second line contains `n` space-separated integers representing the bean price on each day.

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
