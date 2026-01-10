## Title
Laser Tag Game

## Slug
laser-tag-game

## Difficulty
Easy

## Description
An arena logs player active times.

The game system records the activation and deactivation of every player in two integer arrays, `startTime` and `endTime`. The $i$-th player enters the arena at `startTime[i]` and exits at `endTime[i]`, inclusive.

The referee wants to know how many players were playing during a specific power hour `[queryStart, queryEnd]`. A player is considered playing if their match overlaps with the power hour at any point (even for a single moment).

Your task is to return the total number of players who were playing during the given power hour.

## Examples

### 1

#### Input
3
1 2 3
3 2 7
2 4

#### Output
3

#### Explanation
The power hour is `[2, 4]`.
- Player 1 `[1, 3]` overlaps with `[2, 4]` (times 2, 3).
- Player 2 `[2, 2]` overlaps with `[2, 4]` (time 2).
- Player 3 `[3, 7]` overlaps with `[2, 4]` (times 3, 4).
All 3 players were playing.

### 2

#### Input
1
4
4
1 3

#### Output
0

#### Explanation
The player was playing at time `[4, 4]`. The power hour is `[1, 3]`. There is no overlap.

## Input Format
- The first line contains an integer `n`, the number of players.
- The second line contains `n` space-separated integers for `startTime`.
- The third line contains `n` space-separated integers for `endTime`.
- The fourth line contains two integers, `queryStart` and `queryEnd`.

## Output Format
- Return a single integer representing the number of players playing during the power hour.

## Constraints
- 1 ≤ n ≤ 10^5
- 1 ≤ startTime[i] ≤ endTime[i] ≤ 10^9
- 1 ≤ queryStart ≤ queryEnd ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, interval, linear-scan

## Company
amazon
