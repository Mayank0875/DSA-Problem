## Title

Player Consistency XOR Metric

## Slug

player-consistency-xor-metric

## Difficulty

Easy

## Description

A sports analyst tracks a player's performance metric (e.g., points scored) over N games: A₁, A₂, ..., Aₙ. To measure consistency over K-game stretches, they use a sliding window. For each window, a consistency score is calculated by XORing the player's metrics within that window. To derive a single overall consistency metric for the season, all the window scores are XORed together. Calculate this final consistency metric for the player.

## Examples

### 1

#### Input

5 3
[1, 2, 3, 4, 5]

#### Output

7

#### Explanation

Performance windows of size 3:
    •   [1, 2, 3] → Score (XOR) = 0
    •   [2, 3, 4] → Score (XOR) = 5
    •   [3, 4, 5] → Score (XOR) = 2

Final Consistency Metric = 0 ^ 5 ^ 2 = 7

### 2

#### Input

4 2
[5, 1, 3, 2]

#### Output

7

#### Explanation

Windows:
    •   [5, 1] → XOR = 4
    •   [1, 3] → XOR = 2
    •   [3, 2] → XOR = 1

Final Consistency Metric = 4 ^ 2 ^ 1 = 7

## Input Format

- The first line contains two integers N (number of games) and K (window size).
- The second line contains N space-separated integers — the performance metrics.

## Output Format

- Return a single integer — the final consistency metric.

## Constraints

- 1 ≤ N ≤ 10^5
- 1 ≤ K ≤ N
- 0 ≤ arr[i] ≤ 1e9

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

arrays, sliding window, sports analytics, bit manipulation