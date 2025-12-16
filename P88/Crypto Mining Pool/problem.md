## Title
Crypto Mining Pool

## Slug
crypto-mining-pool

## Difficulty
Medium

## Description
Miners have different hashrates. To solve a block first, a pool needs more than half the total network hashrate.

Your task is to count the number of **poolss**. A pool is considered valid if it satisfies two specific criteria:
1.  **Block Solution:** The total hashrate of the pool is strictly greater than half of the total hashrate across all miners.
2.  **No Superfluous miners:** The pool is minimal. This means that removing **any one** miner from the pool would cause the remaining total to drop to half or less of the total hashrate (losing the Block Solution).

## Examples

### 1

#### Input
5
3 1 4 1 5

#### Output
4

#### Explanation
Total hashrate is 14. Half is 7. We need a sum > 7.
The group {5, 4, 1} (Sum 10) is **not** valid because removing 1 leaves 9, which is still > 7.
Valid groups are those where every member is critical.

### 2

#### Input
4
1 2 3 4

#### Output
3

#### Explanation
Total hashrate = 10. Half = 5.
Valid poolss: {4, 2}, {4, 3}, {3, 2, 1}.

## Input Format
- The first line contains an integer n: the number of miners.
- The second line contains n integers: the hashrate of each miner.

## Output Format
- Return one integer: the total number of valid poolss.

## Constraints
- 1 ≤ n ≤ 60
- 1 ≤ hashrate ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths, dynamic-programming
