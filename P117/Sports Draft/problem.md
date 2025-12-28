## Title
Sports Draft

## Slug
sports-draft

## Difficulty
Medium

## Description
Athletes are drafted. The First Team picks the star, the Second Team (you) picks the solid player, and the Benchwarmers get the rest.

There are $3n$ players of varying skill rating available. The distribution follows a strict protocol. In each round, you must select any 3 players. The parties then claim them based on the following rules:

1. The **First Team** takes the player with the **maximum** skill rating from the triplet.
2. You, the **Second Team**, take the player with the **second maximum** skill rating.
3. The **Benchwarmers** takes the remaining player (the one with the minimum skill rating).

This process repeats until all players are distributed. Your goal as the Second Team is to maximize the total skill rating of the players you acquire.

Given an array of integers `ratings`, where `ratings[i]` represents the skill rating of the $i$-th player, return the maximum total skill rating you can obtain.

## Examples

### 1

#### Input
6
2 4 1 2 7 8

#### Output
9

#### Explanation
You have 6 players. One optimal strategy is:
1. Pick the triplet `(2, 7, 8)`. First Team takes `8`, you take `7`, Benchwarmers takes `2`.
2. Pick the remaining `(1, 2, 4)`. First Team takes `4`, you take `2`, Benchwarmers takes `1`.
Total skill rating = $7 + 2 = 9$.

### 2

#### Input
3
2 4 5

#### Output
4

#### Explanation
There is only one triplet `(2, 4, 5)`. First Team takes `5`, you take `4`, Benchwarmers takes `2`. Total = 4.

## Input Format
- The first line contains a single integer $3n$, the number of players.
- The second line contains $3n$ space-separated integers representing the `ratings` array.

## Output Format
- Return a single integer representing the maximum total skill rating you can collect.

## Constraints
- 1 ≤ ratings.length ≤ 10^5
- `ratings.length` is divisible by 3.
- 1 ≤ ratings[i] ≤ 10^4

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, sorting, greedy, math
