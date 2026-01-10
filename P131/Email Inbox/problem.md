## Title
Email Inbox

## Slug
email-inbox

## Difficulty
Medium

## Description
You are deleting old emails. You select and delete a batch of emails equal to a digit of the total unread count.

You start with a **unread count** of `n`. The goal is to reduce this unread count to exactly 0.

In one **deletion batch**, you can look at the digits of the current unread count, choose one **non-zero digit**, and subtract it from the current unread count.

For example, if the unread count is 27, the digits are 2 and 7. You can subtract 2 (getting 25) or 7 (getting 20).

Your task is to find the **minimum** number of deletion batchs required to reduce the unread count to 0.

## Examples

### 1

#### Input
27

#### Output
5

#### Explanation
1. 27 - 7 = 20
2. 20 - 2 = 18
3. 18 - 8 = 10
4. 10 - 1 = 9
5. 9 - 9 = 0
Total deletion batchs: 5.

### 2

#### Input
0

#### Output
0

#### Explanation
The unread count is already 0.

## Input Format
- The input contains a single integer `n`.

## Output Format
- Return a single integer representing the minimum number of deletion batchs.

## Constraints
- 0 ≤ n ≤ 10^6

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, greedy, math, bfs
