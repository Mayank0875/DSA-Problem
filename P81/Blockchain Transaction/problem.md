## Title
Blockchain Transaction

## Slug
blockchain-transaction

## Difficulty
Medium

## Description
Funds move from Wallet 1 to Wallet n.

The blockchain has `n` wallets and `m` directed transfers. Transfers may repeat between the same pair of wallets and self-loops are allowed. A transaction history of length `k` is a sequence of exactly `k` directed transfers; wallets and transfers may be visited multiple times.

Given `n`, `m`, `k` and a list of the `m` directed transfers (each transfer given as two integers `u` `v` meaning a directed transfer from `u` to `v`), compute the number of distinct transaction histories that start at wallet 1 and end at wallet `n` with length exactly `k`. Output the answer modulo 1000000007.

## Examples

### 1

#### Input
3 4 8
1 2
2 3
3 1
3 2

#### Output
2

#### Explanation
We have 3 wallets. We want the number of directed transaction histories of length 8 from wallet 1 to wallet 3.
Valid length-8 transaction histories:
1 -> 2 -> 3 -> 1 -> 2 -> 3 -> 1 -> 2 -> 3
1 -> 2 -> 3 -> 2 -> 3 -> 1 -> 2 -> 3
There are 2 such transaction histories.

### 2

#### Input
3 4 2
1 2
2 3
3 1
3 2

#### Output
1

#### Explanation
Assuming the graph has transfers 1->2 and 2->3, the only transaction history of length 2 from wallet 1 to wallet 3 is:
1 -> 2 -> 3

## Input Format
- The first line contains three integers n, m, and k: the number of wallets, transfers, and the required transaction history length.
- The next m lines describe the transfers. Each line contains two integers u and v, indicating a directed transfer from wallet u to wallet v.

## Output Format
- Return single integer: the number of transaction histories modulo 10^9+7.

## Constraints
- 1 ≤ n ≤ 100
- 1 ≤ m ≤ 10^5
- 1 ≤ k ≤ 10^18
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph, dynamic-programming
