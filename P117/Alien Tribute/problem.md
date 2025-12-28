## Title
Alien Tribute

## Slug
alien-tribute

## Difficulty
Medium

## Description
Resources are offered to invaders. The Overlords take the uranium, the Collaborators (you) take the steel, and the Rebels take the scraps.

There are $3n$ ingots of varying density available. The distribution follows a strict protocol. In each round, you must select any 3 ingots. The parties then claim them based on the following rules:

1. The **Overlords** takes the ingot with the **maximum** density from the triplet.
2. You, the **Collaborators**, take the ingot with the **second maximum** density.
3. The **Rebels** takes the remaining ingot (the one with the minimum density).

This process repeats until all ingots are distributed. Your goal as the Collaborators is to maximize the total density of the ingots you acquire.

Given an array of integers `ingots`, where `ingots[i]` represents the density of the $i$-th ingot, return the maximum total density you can obtain.

## Examples

### 1

#### Input
6
2 4 1 2 7 8

#### Output
9

#### Explanation
You have 6 ingots. One optimal strategy is:
1. Pick the triplet `(2, 7, 8)`. Overlords takes `8`, you take `7`, Rebels takes `2`.
2. Pick the remaining `(1, 2, 4)`. Overlords takes `4`, you take `2`, Rebels takes `1`.
Total density = $7 + 2 = 9$.

### 2

#### Input
3
2 4 5

#### Output
4

#### Explanation
There is only one triplet `(2, 4, 5)`. Overlords takes `5`, you take `4`, Rebels takes `2`. Total = 4.

## Input Format
- The first line contains a single integer $3n$, the number of ingots.
- The second line contains $3n$ space-separated integers representing the `ingots` array.

## Output Format
- Return a single integer representing the maximum total density you can collect.

## Constraints
- 1 ≤ ingots.length ≤ 10^5
- `ingots.length` is divisible by 3.
- 1 ≤ ingots[i] ≤ 10^4

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, sorting, greedy, math
