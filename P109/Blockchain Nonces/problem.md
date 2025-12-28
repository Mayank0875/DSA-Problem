## Title
Blockchain Nonces

## Slug
blockchain-nonces

## Difficulty
Easy

## Description
A miner validates a block of transactions. Duplicate transaction nonces are invalid and must be rejected.

Your task is to determine if any nonce appears at least twice in the list.

## Examples

### 1

#### Input
4
1 2 3 1

#### Output
Yes

#### Explanation
The nonce `1` appears twice.

### 2

#### Input
4
1 2 3 4

#### Output
No

#### Explanation
All nonces are distinct.

## Input Format
- The first line contains a single integer n, the number of transactions.
- The second line contains n space-separated integers, representing the nonces.

## Output Format
- Return `Yes` if any nonce appears at least twice, otherwise `No`.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ values ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
sorting, array, hash-table
