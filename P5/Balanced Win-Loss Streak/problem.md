## Title

Balanced Win-Loss Streak

## Slug

balanced-win-loss-streak

## Difficulty

Easy

## Description

A sports team's season results are recorded as a sequence, where '1' denotes a win and '0' denotes a loss. The coach wants to find the longest continuous stretch of games during the season where the team had exactly as many wins as losses. This indicates a period of balanced performance. Given the sequence of game outcomes, determine the length of the longest balanced win-loss streak.

## Examples

### 1

#### Input

2
[0, 1]

#### Output

2

#### Explanation

The streak [0, 1] (Loss, Win) is the longest balanced streak.

### 2

#### Input

3
[0, 1, 0]

#### Output

2

#### Explanation

[0, 1] (Loss, Win) and [1, 0] (Win, Loss) are the longest balanced streaks.

## Input Format

- The first line contains a single integer N, the number of games played.
- The second line contains N space-separated integers, where 0 is a loss and 1 is a win.

## Output Format

- Return a single integer representing the length of the longest contiguous streak with an equal number of 0s and 1s.

## Constraints

- 1 ≤ N ≤ 10^5
- 0 ≤ arr[i] ≤ 1

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

arrays, sports analytics, prefix sum, hashmap