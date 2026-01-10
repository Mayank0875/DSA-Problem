## Title
Online Gamer Activity

## Slug
online-gamer-activity

## Difficulty
Easy

## Description
A game server logs session times for players.

The server log records the login time and logout time of every player in two integer arrays, `startTime` and `endTime`. The $i$-th player logs in at `startTime[i]` and logs out at `endTime[i]`, inclusive.

The game dev wants to know how many players were online during a specific server event `[queryStart, queryEnd]`. A player is considered online if their session overlaps with the server event at any point (even for a single moment).

Your task is to return the total number of players who were online during the given server event.

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
The server event is `[2, 4]`.
- Player 1 `[1, 3]` overlaps with `[2, 4]` (times 2, 3).
- Player 2 `[2, 2]` overlaps with `[2, 4]` (time 2).
- Player 3 `[3, 7]` overlaps with `[2, 4]` (times 3, 4).
All 3 players were online.

### 2

#### Input
1
4
4
1 3

#### Output
0

#### Explanation
The player was online at time `[4, 4]`. The server event is `[1, 3]`. There is no overlap.

## Input Format
- The first line contains an integer `n`, the number of players.
- The second line contains `n` space-separated integers for `startTime`.
- The third line contains `n` space-separated integers for `endTime`.
- The fourth line contains two integers, `queryStart` and `queryEnd`.

## Output Format
- Return a single integer representing the number of players online during the server event.

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
