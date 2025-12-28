## Title
Bank Account Setup

## Slug
bank-account-setup

## Difficulty
Easy

## Description
A batch job creates new accounts. It must ensure no two accounts in the batch were assigned the same account number by mistake.

Your task is to determine if any account number appears at least twice in the list.

## Examples

### 1

#### Input
4
1 2 3 1

#### Output
Yes

#### Explanation
The account number `1` appears twice.

### 2

#### Input
4
1 2 3 4

#### Output
No

#### Explanation
All account numbers are distinct.

## Input Format
- The first line contains a single integer n, the number of new accounts.
- The second line contains n space-separated integers, representing the account numbers.

## Output Format
- Return `Yes` if any account number appears at least twice, otherwise `No`.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ values ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
sorting, array, hash-table
