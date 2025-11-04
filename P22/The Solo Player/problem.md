## Title

The Solo Player

## Slug

solo-player

## Difficulty

Medium

## Description

In a tournament, players are listed and sorted by their rank. Every player is scheduled for a 1v1 match, so their rank should appear twice in the list (once for each player in the match-up). However, one player received a "bye" and has no opponent; their rank appears only once. Find the rank of this solo player.

You must write an algorithm with O(log n) runtime complexity.

## Examples

### 1

#### Input

9 
[1, 1, 2, 3, 3, 4, 4, 8, 8]


#### Output

2

#### Explanation

In the sequence [1, 1, 2, 3, 3, 4, 4, 8, 8], the number 2 appears only once.

### 2

#### Input

7 
[3, 3, 7, 7, 10, 11, 11]

#### Output

10

#### Explanation

In the sequence [3, 3, 7, 7, 10, 11, 11], the number 10 appears only once.

## Input Format

- The first line contains an odd integer n, the total number of player entries.
- The second line contains n space-separated integers representing the sorted player ranks.

## Output Format

- Return a single integer: the rank of the player that appears only once.

## Constraints

- 1 ≤ n ≤ 10^5
- 1 ≤ stone_value ≤ 10^9
- The array is sorted.
- Every element appears twice except for one.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

binary-search, array