## Title
Chocolatier

## Slug
chocolatier

## Difficulty
Medium

## Description
Batches are finished. The Truffles go to the display, the Bars (you) go to the shelf, and the Scraps go to the bin.

There are $3n$ batches of varying cocoa % available. The distribution follows a strict protocol. In each round, you must select any 3 batches. The parties then claim them based on the following rules:

1. The **Display** takes the batch with the **maximum** cocoa % from the triplet.
2. You, the **Shelf**, take the batch with the **second maximum** cocoa %.
3. The **Bin** takes the remaining batch (the one with the minimum cocoa %).

This process repeats until all batches are distributed. Your goal as the Shelf is to maximize the total cocoa % of the batches you acquire.

Given an array of integers `batches`, where `batches[i]` represents the cocoa % of the $i$-th batch, return the maximum total cocoa % you can obtain.

## Examples

### 1

#### Input
6
2 4 1 2 7 8

#### Output
9

#### Explanation
You have 6 batches. One optimal strategy is:
1. Pick the triplet `(2, 7, 8)`. Display takes `8`, you take `7`, Bin takes `2`.
2. Pick the remaining `(1, 2, 4)`. Display takes `4`, you take `2`, Bin takes `1`.
Total cocoa % = $7 + 2 = 9$.

### 2

#### Input
3
2 4 5

#### Output
4

#### Explanation
There is only one triplet `(2, 4, 5)`. Display takes `5`, you take `4`, Bin takes `2`. Total = 4.

## Input Format
- The first line contains a single integer $3n$, the number of batches.
- The second line contains $3n$ space-separated integers representing the `batches` array.

## Output Format
- Return a single integer representing the maximum total cocoa % you can collect.

## Constraints
- 1 ≤ batches.length ≤ 10^5
- `batches.length` is divisible by 3.
- 1 ≤ batches[i] ≤ 10^4

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, sorting, greedy, math
