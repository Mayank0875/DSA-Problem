## Title
Stock Market Flow

## Slug
stock-market-flow

## Difficulty
Medium

## Description
Capital flows from the Investor (node 1) to the Asset (node n) through intermediaries.

The market has `n` accounts and `m` directed transactions. Transactions may repeat between the same pair of accounts and self-loops are allowed. A flow of length `k` is a sequence of exactly `k` directed transactions; accounts and transactions may be visited multiple times.

Given `n`, `m`, `k` and a list of the `m` directed transactions (each transaction given as two integers `u` `v` meaning a directed transaction from `u` to `v`), compute the number of distinct flows that start at account 1 and end at account `n` with length exactly `k`. Output the answer modulo 1000000007.

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
We have 3 accounts. We want the number of directed flows of length 8 from account 1 to account 3.
Valid length-8 flows:
1 -> 2 -> 3 -> 1 -> 2 -> 3 -> 1 -> 2 -> 3
1 -> 2 -> 3 -> 2 -> 3 -> 1 -> 2 -> 3
There are 2 such flows.

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
Assuming the graph has transactions 1->2 and 2->3, the only flow of length 2 from account 1 to account 3 is:
1 -> 2 -> 3

## Input Format
- The first line contains three integers n, m, and k: the number of accounts, transactions, and the required flow length.
- The next m lines describe the transactions. Each line contains two integers u and v, indicating a directed transaction from account u to account v.

## Output Format
- Return single integer: the number of flows modulo 10^9+7.

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
