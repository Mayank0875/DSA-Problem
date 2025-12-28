## Title
University Housing

## Slug
university-housing

## Difficulty
Medium

## Description
Dorm rooms are assigned. Seniors get the penthouses, Juniors (you) get the suites, and Freshmen get the closets.

There are $3n$ rooms of varying square footage available. The distribution follows a strict protocol. In each round, you must select any 3 rooms. The parties then claim them based on the following rules:

1. The **Seniors** takes the room with the **maximum** square footage from the triplet.
2. You, the **Juniors**, take the room with the **second maximum** square footage.
3. The **Freshmen** takes the remaining room (the one with the minimum square footage).

This process repeats until all rooms are distributed. Your goal as the Juniors is to maximize the total square footage of the rooms you acquire.

Given an array of integers `sizes`, where `sizes[i]` represents the square footage of the $i$-th room, return the maximum total square footage you can obtain.

## Examples

### 1

#### Input
6
2 4 1 2 7 8

#### Output
9

#### Explanation
You have 6 rooms. One optimal strategy is:
1. Pick the triplet `(2, 7, 8)`. Seniors takes `8`, you take `7`, Freshmen takes `2`.
2. Pick the remaining `(1, 2, 4)`. Seniors takes `4`, you take `2`, Freshmen takes `1`.
Total square footage = $7 + 2 = 9$.

### 2

#### Input
3
2 4 5

#### Output
4

#### Explanation
There is only one triplet `(2, 4, 5)`. Seniors takes `5`, you take `4`, Freshmen takes `2`. Total = 4.

## Input Format
- The first line contains a single integer $3n$, the number of rooms.
- The second line contains $3n$ space-separated integers representing the `sizes` array.

## Output Format
- Return a single integer representing the maximum total square footage you can collect.

## Constraints
- 1 ≤ sizes.length ≤ 10^5
- `sizes.length` is divisible by 3.
- 1 ≤ sizes[i] ≤ 10^4

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, sorting, greedy, math
