## Title

The Trader's Profit

## Slug

the-traders-profit

## Difficulty

Medium

## Description

In a distant galaxy, three factions—the Hegemony, the Traders (you), and the Scavengers—have agreed to a treaty for distributing resource canisters found on new planets. There are $3n$ canisters of varying value scattered across a sector.

The distribution follows a strict protocol. In each round, you must select any 3 canisters. The factions then claim them based on the following rules:
1. The **Hegemony**, being the most powerful, takes the canister with the **maximum** value from the triplet.
2. You, the **Trader**, take the canister with the **second maximum** value.
3. The **Scavenger** takes the remaining canister (the one with the minimum value).

This process repeats until all canisters are distributed. Your goal as the Trader is to maximize the total value of the canisters you acquire.

Given an array of integers `canisters`, where `canisters[i]` represents the value of the $i$-th canister, return the maximum total value you can obtain.

## Examples

### 1

#### Input

6
2 4 1 2 7 8

#### Output

9

#### Explanation

You have 6 canisters. One optimal strategy is:
1. Pick the triplet `(2, 7, 8)`. Hegemony takes `8`, you take `7`, Scavengers take `2`.
2. Pick the remaining `(1, 2, 4)`. Hegemony takes `4`, you take `2`, Scavengers take `1`.
Total value = $7 + 2 = 9$.
    
### 2

#### Input

3
2 4 5

#### Output

5

#### Explanation

There is only one triplet `(2, 4, 5)`. Hegemony takes `5`, you take `4`, Scavengers take `2`. Total = 4.
  

## Input Format  

- The first line contains a single integer $3n$, the number of canisters.
- The second line contains $3n$ space-separated integers representing the `canisters` array.

## Output Format  

- Return a single integer representing the maximum total value you can collect.
  

## Constraints  

- 1 ≤ canisters.length ≤ 1e5
- `canisters.length` is divisible by 3.
- 1 ≤ canister[i] ≤ 1e4


## Time Limit

2 second

## Memory Limit

256 MB

## Tags

array, sorting, greedy