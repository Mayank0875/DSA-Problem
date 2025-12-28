## Title
NFT Flipper

## Slug
nft-flipper

## Difficulty
Easy

## Description
A digital artist watches the floor price of a Bored Ape collection. They want to buy one ape and flip it.

You have a list of floor price for $n$ consecutive hours. You want to make one perfect move: mint on one hour and list on a different hour in the future. You cannot list before you mint.

Your goal is to find the **maximum possible ETH gained** you can earn from this single transaction. If it is impossible to make any ETH gained (i.e., the floor price only goes down), you should return 0.

## Examples

### 1

#### Input
6
7 1 5 3 6 4

#### Output
5

#### Explanation
mint on hour 2 (floor price = 1) and list on hour 5 (floor price = 6). The ETH gained is $6 - 1 = 5$.
Note that minting on hour 1 (floor price = 7) is not optimal, as all future values are lower.

### 2

#### Input
5
7 6 4 3 1

#### Output
0

#### Explanation
The floor price never increases, so it is impossible to make a ETH gained. The maximum ETH gained is 0.

## Input Format
- The first line contains a single integer `n`, the number of hours.
- The second line contains `n` space-separated integers representing the floor price on each hour.

## Output Format
- Return a single integer representing the maximum ETH gained. If no ETH gained can be made, return 0.

## Constraints
- 1 ≤ n ≤ 10^5
- 0 ≤ values ≤ 10^4

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, dynamic-programming, greedy
