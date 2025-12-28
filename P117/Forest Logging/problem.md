## Title
Forest Logging

## Slug
forest-logging

## Difficulty
Medium

## Description
Logs are sorted at the mill. The Furniture Maker takes the mahogany, the Paper Mill (you) takes the pine, and the rest becomes Firewood.

There are $3n$ logs of varying wood quality available. The distribution follows a strict protocol. In each round, you must select any 3 logs. The parties then claim them based on the following rules:

1. The **Furniture Maker** takes the log with the **maximum** wood quality from the triplet.
2. You, the **Paper Mill**, take the log with the **second maximum** wood quality.
3. The **Firewood** takes the remaining log (the one with the minimum wood quality).

This process repeats until all logs are distributed. Your goal as the Paper Mill is to maximize the total wood quality of the logs you acquire.

Given an array of integers `logs`, where `logs[i]` represents the wood quality of the $i$-th log, return the maximum total wood quality you can obtain.

## Examples

### 1

#### Input
6
2 4 1 2 7 8

#### Output
9

#### Explanation
You have 6 logs. One optimal strategy is:
1. Pick the triplet `(2, 7, 8)`. Furniture Maker takes `8`, you take `7`, Firewood takes `2`.
2. Pick the remaining `(1, 2, 4)`. Furniture Maker takes `4`, you take `2`, Firewood takes `1`.
Total wood quality = $7 + 2 = 9$.

### 2

#### Input
3
2 4 5

#### Output
4

#### Explanation
There is only one triplet `(2, 4, 5)`. Furniture Maker takes `5`, you take `4`, Firewood takes `2`. Total = 4.

## Input Format
- The first line contains a single integer $3n$, the number of logs.
- The second line contains $3n$ space-separated integers representing the `logs` array.

## Output Format
- Return a single integer representing the maximum total wood quality you can collect.

## Constraints
- 1 ≤ logs.length ≤ 10^5
- `logs.length` is divisible by 3.
- 1 ≤ logs[i] ≤ 10^4

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, sorting, greedy, math
