## Title
Golf Tournament

## Slug
golf-tournament

## Difficulty
Easy

## Description
A local golf club is finalizing the leaderboard for a tournament.

The caddy records the score of $N$ players in an array. To award prizes, the organizer needs to assign a rank to every player based on its score.

The ranking rules are simple: the player with the **smallest** score gets **Rank 1**. The next distinct score gets **Rank 2**, and so on.

If two or more players have the exact same score, they must receive the **same rank**. The ranks must be integers starting from 1.

Your task is to replace each player's score with its corresponding rank.

## Examples

### 1

#### Input
4
40 10 20 30

#### Output
4 1 2 3

#### Explanation
10 is the smallest (Rank 1). 20 is the second smallest (Rank 2). 30 is third (Rank 3). 40 is largest (Rank 4).

### 2

#### Input
3
2 2 2

#### Output
1 1 1

#### Explanation
All players share the same score, so they share Rank 1.

## Input Format
- The first line contains an integer `n`, the number of players.
- The second line contains `n` space-separated integers representing the scores.

## Output Format
- Return an array of integers where each element is the rank of the corresponding player.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ values ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, hash-table, sorting
