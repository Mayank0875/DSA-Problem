## Title
Crypto Wallets

## Slug
crypto-wallets

## Difficulty
Hard

## Description
Tokens are bundled into transactions. The asset class of a transaction is the most frequent token ID included.

Satoshi has a collection of $n$ tokens, where each token is represented by an integer ID.

To audit the blockchain, Satoshi must partition these tokens into several non-empty transactions. Every token from the original collection must belong to exactly one transaction. From each transaction, a "asset class" is extracted. The asset class is defined as the **mode** (most frequent element) of the tokens in that transaction. If a transaction has multiple tokens tied for the most frequent appearance, any one of them can be chosen as the asset class.

Satoshi collects all the extracted asset classs to form a final multiset. Your task is to calculate how many distinct final multisets can be created using this process. Two multisets are considered different if the frequency of any ID differs between them.

## Examples

### 1

#### Input
3
1 2 3

#### Output
7

#### Explanation
Any non-empty subset of {1, 2, 3} can be achieved, for a total of 7 multisets.

### 2

#### Input
3
1 2 2

#### Output
4

#### Explanation
We can generate 4 different multisets:
1. Partition into {1, 2, 2} -> asset class is 2 -> Result {2}.
2. Partition into {1, 2}, {2} -> asset classs 1, 2 or 2, 2 -> Result {1, 2} or {2, 2}. (Wait, if {1, 2} mode can be 1 or 2. If we pick 2, result is {2, 2}).
3. Partition into {1}, {2, 2} -> asset classs 1, 2 -> Result {1, 2}.
4. Partition into {1}, {2}, {2} -> asset classs 1, 2, 2 -> Result {1, 2, 2}.
Total distinct multisets: {2}, {2, 2}, {1, 2}, {1, 2, 2}.

## Input Format
- The first line contains an integer $n$, the number of tokens.
- The second line contains $n$ space-separated integers representing the token IDs.

## Output Format
- Return a single integer representing the number of different multisets of asset classs possible, modulo $998244353$.

## Constraints
- 1 ≤ n ≤ 5000
- 1 ≤ ID ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, math, combinatorics
