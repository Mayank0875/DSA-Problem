## Title

Lost Signal: Nearest Stronger Transmission

## Slug

lost-signal-nearest-stronger-transmission

## Difficulty

Easy

## Description

Imagine a series of communication towers along a remote road, each broadcasting a signal of varying strength. As you move past each tower, you look back (to your left) and want to know the strength of the nearest tower that is broadcasting a strictly stronger signal than the one you are currently at. If all previous towers have weaker or equal signal strength, or if it's the first tower, there is no such stronger tower to the left. Your goal is to determine this stronger tower's signal strength for each position along the road.

## Examples

### 1

#### Input

8
[30, 60, 90, 50, 80, 40, 70, 50]

#### Output

[-1, -1, -1, 90, 90, 80, 80, 70]

#### Explanation

Tower 0 (30): No previous tower. Output -1.
Tower 1 (60): Tower 0 (30) is weaker. Output -1.
Tower 2 (90): Towers 0 (30), 1 (60) are weaker. Output -1.
Tower 3 (50): Tower 2 (90) is the nearest stronger. Output 90.
Tower 4 (80): Tower 2 (90) is the nearest stronger. Output 90.
Tower 5 (40): Tower 4 (80) is the nearest stronger. Output 80.
Tower 6 (70): Tower 4 (80) is the nearest stronger. Output 80.
Tower 7 (50): Tower 6 (70) is the nearest stronger. Output 70.

### 2

#### Input

5
50 50 50 50 50

#### Output

[-1, -1, -1, -1, -1]

#### Explanation

All towers broadcast the same strength, so no strictly stronger previous tower exists.

## Input Format

The first line contains a single integer n, the number of towers.
The second line contains n space-separated integers h_0, h_1, ..., h_[n-1], representing the signal strength of each tower.

## Output Format

Return array of integers. The i-th integer should be the strength of the nearest tower j < i such that h_j > h_i. If no such day exists, then -1.

## Constraints

1 ≤ n ≤ 10^5
1 ≤ h_i ≤ 10^9 for all 0 ≤ i < n.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

stack, array