## Title
Movie Roles

## Slug
movie-roles

## Difficulty
Medium

## Description
Scripts are handed out. The Lead gets the hero, the Supporting Actor (you) gets the sidekick, and the Extra gets the background.

There are $3n$ roles of varying lines count available. The distribution follows a strict protocol. In each round, you must select any 3 roles. The parties then claim them based on the following rules:

1. The **Lead** takes the role with the **maximum** lines count from the triplet.
2. You, the **Supporting**, take the role with the **second maximum** lines count.
3. The **Extra** takes the remaining role (the one with the minimum lines count).

This process repeats until all roles are distributed. Your goal as the Supporting is to maximize the total lines count of the roles you acquire.

Given an array of integers `lines`, where `lines[i]` represents the lines count of the $i$-th role, return the maximum total lines count you can obtain.

## Examples

### 1

#### Input
6
2 4 1 2 7 8

#### Output
9

#### Explanation
You have 6 roles. One optimal strategy is:
1. Pick the triplet `(2, 7, 8)`. Lead takes `8`, you take `7`, Extra takes `2`.
2. Pick the remaining `(1, 2, 4)`. Lead takes `4`, you take `2`, Extra takes `1`.
Total lines count = $7 + 2 = 9$.

### 2

#### Input
3
2 4 5

#### Output
4

#### Explanation
There is only one triplet `(2, 4, 5)`. Lead takes `5`, you take `4`, Extra takes `2`. Total = 4.

## Input Format
- The first line contains a single integer $3n$, the number of roles.
- The second line contains $3n$ space-separated integers representing the `lines` array.

## Output Format
- Return a single integer representing the maximum total lines count you can collect.

## Constraints
- 1 ≤ lines.length ≤ 10^5
- `lines.length` is divisible by 3.
- 1 ≤ lines[i] ≤ 10^4

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, sorting, greedy, math
