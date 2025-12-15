## Title
Crypto Currency Mixing

## Slug
crypto-currency-mixing

## Difficulty
Medium

## Description
To anonymize funds, a transaction is forwarded exactly k times through different wallets. Each transfer incurs a fee.

You need to find a path from Input Wallet (index 1) to Output Wallet (index n) that consists of **exactly** `k` transfers.
Each transfer connects a source wallet to a destination wallet and has a specific fee associated with it.

Your goal is to calculate the minimum total fee required to travel from Input Wallet to Output Wallet using exactly `k` transfers. If it is impossible to reach the destination with exactly `k` transfers, return -1.

## Examples

### 1

#### Input
3 4 8
1 2 5
2 3 4
3 1 1
3 2 2

#### Output
27

#### Explanation
We need a path from Input Wallet to Output Wallet using exactly 8 transfers.
Consider the path: 1 -> 2 -> 3 -> 2 -> 3 -> 2 -> 3 -> 2 -> 3.
Costs: 5 + 4 + 2 + 4 + 2 + 4 + 2 + 4 = 27.
This is the minimum cost possible.

### 2

#### Input
2 1 100
1 2 10

#### Output
-1

#### Explanation
There is only one transfer from 1 to 2. It is impossible to make 100 transfers because once you reach node 2, there are no outgoing transfers to continue.

## Input Format
- The first line contains three integers `n`, `m`, and `k`: the number of wallets, transfers, and the required number of jumps.
- The next `m` lines describe the transfers. Each line contains three integers `u`, `v`, and `w`: a transfer from `u` to `v` with fee `w`.

## Output Format
- Return one integer: the minimum total fee. If no such path exists, return -1.

## Constraints
- 1 ≤ n ≤ 100
- 1 ≤ m ≤ n * (n - 1)
- 1 ≤ k ≤ 10^9
- 1 ≤ u, v ≤ n
- 1 ≤ w ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph, dynamic-programming
