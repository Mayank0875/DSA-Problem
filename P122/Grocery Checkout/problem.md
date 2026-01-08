## Title
Grocery Checkout

## Slug
grocery-checkout

## Difficulty
Hard

## Description
A cashier scans items. They scan 1 item or a 'buy one get one' pair (2 items).

The cashier starts at item 0 and wishes to reach item $n$. On each move, The cashier can scan forward either **1 item** or **2 items**.

Your task is to calculate the total number of distinct ways to reach exactly item $n$. Since the distance $n$ can be extremely large, return the answer modulo $10^9 + 7$.

## Examples

### 1

#### Input
2

#### Output
2

#### Explanation
There are two ways to reach item 2:
1. 1 item + 1 item
2. 2 items

### 2

#### Input
3

#### Output
3

#### Explanation
There are three ways:
1. 1 + 1 + 1
2. 1 + 2
3. 2 + 1

## Input Format
- The only input line has an integer $n$ — the target item.

## Output Format
- Return a single integer: the number of ways modulo $10^9 + 7$.

## Constraints
- 1 ≤ n ≤ 10^18

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, math

