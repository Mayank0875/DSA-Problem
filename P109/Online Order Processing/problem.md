## Title
Online Order Processing

## Slug
online-order-processing

## Difficulty
Easy

## Description
An e-commerce system processes orders. Duplicate Order IDs in the daily batch file indicate a database synchronization issue.

Your task is to determine if any order ID appears at least twice in the list.

## Examples

### 1

#### Input
4
1 2 3 1

#### Output
Yes

#### Explanation
The order ID `1` appears twice.

### 2

#### Input
4
1 2 3 4

#### Output
No

#### Explanation
All order IDs are distinct.

## Input Format
- The first line contains a single integer n, the number of orders.
- The second line contains n space-separated integers, representing the order IDs.

## Output Format
- Return `Yes` if any order ID appears at least twice, otherwise `No`.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ values ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
sorting, array, hash-table
