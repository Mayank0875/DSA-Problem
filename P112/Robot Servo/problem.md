## Title
Robot Servo

## Slug
robot-servo

## Difficulty
Easy

## Description
A robotics club tracks servo motor prices. They want to buy a batch cheap and sell them during the competition season.

You have a list of motor price for $n$ consecutive weeks. You want to make one perfect move: order on one week and distribute on a different week in the future. You cannot distribute before you order.

Your goal is to find the **maximum possible fundraising** you can earn from this single transaction. If it is impossible to make any fundraising (i.e., the motor price only goes down), you should return 0.

## Examples

### 1

#### Input
6
7 1 5 3 6 4

#### Output
5

#### Explanation
order on week 2 (motor price = 1) and distribute on week 5 (motor price = 6). The fundraising is $6 - 1 = 5$.
Note that ordering on week 1 (motor price = 7) is not optimal, as all future values are lower.

### 2

#### Input
5
7 6 4 3 1

#### Output
0

#### Explanation
The motor price never increases, so it is impossible to make a fundraising. The maximum fundraising is 0.

## Input Format
- The first line contains a single integer `n`, the number of weeks.
- The second line contains `n` space-separated integers representing the motor price on each week.

## Output Format
- Return a single integer representing the maximum fundraising. If no fundraising can be made, return 0.

## Constraints
- 1 ≤ n ≤ 10^5
- 0 ≤ values ≤ 10^4

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, dynamic-programming, greedy
