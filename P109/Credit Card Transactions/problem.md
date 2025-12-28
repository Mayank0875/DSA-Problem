## Title
Credit Card Transactions

## Slug
credit-card-transactions

## Difficulty
Easy

## Description
A bank's fraud detection system looks for duplicate transaction IDs within a short time window, which suggests a processing error.

Your task is to determine if any transaction ID appears at least twice in the list.

## Examples

### 1

#### Input
4
1 2 3 1

#### Output
Yes

#### Explanation
The transaction ID `1` appears twice.

### 2

#### Input
4
1 2 3 4

#### Output
No

#### Explanation
All transaction IDs are distinct.

## Input Format
- The first line contains a single integer n, the number of transactions.
- The second line contains n space-separated integers, representing the transaction IDs.

## Output Format
- Return `Yes` if any transaction ID appears at least twice, otherwise `No`.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ values ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
sorting, array, hash-table
