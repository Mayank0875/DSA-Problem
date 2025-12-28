## Title
Shipwreck Salvage

## Slug
shipwreck-salvage

## Difficulty
Medium

## Description
Divers bring up crates. The Government takes the gold bars, the Diver (you) takes the silver coins, and the Historian gets the wood.

There are $3n$ crates of varying market value available. The distribution follows a strict protocol. In each round, you must select any 3 crates. The parties then claim them based on the following rules:

1. The **Government** takes the crate with the **maximum** market value from the triplet.
2. You, the **Diver**, take the crate with the **second maximum** market value.
3. The **Historian** takes the remaining crate (the one with the minimum market value).

This process repeats until all crates are distributed. Your goal as the Diver is to maximize the total market value of the crates you acquire.

Given an array of integers `crates`, where `crates[i]` represents the market value of the $i$-th crate, return the maximum total market value you can obtain.

## Examples

### 1

#### Input
6
2 4 1 2 7 8

#### Output
9

#### Explanation
You have 6 crates. One optimal strategy is:
1. Pick the triplet `(2, 7, 8)`. Government takes `8`, you take `7`, Historian takes `2`.
2. Pick the remaining `(1, 2, 4)`. Government takes `4`, you take `2`, Historian takes `1`.
Total market value = $7 + 2 = 9$.

### 2

#### Input
3
2 4 5

#### Output
4

#### Explanation
There is only one triplet `(2, 4, 5)`. Government takes `5`, you take `4`, Historian takes `2`. Total = 4.

## Input Format
- The first line contains a single integer $3n$, the number of crates.
- The second line contains $3n$ space-separated integers representing the `crates` array.

## Output Format
- Return a single integer representing the maximum total market value you can collect.

## Constraints
- 1 ≤ crates.length ≤ 10^5
- `crates.length` is divisible by 3.
- 1 ≤ crates[i] ≤ 10^4

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, sorting, greedy, math
