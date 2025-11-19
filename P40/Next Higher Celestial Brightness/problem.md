## Title

Next Higher Celestial Brightness

## Slug

next-higher-celestial-brightness

## Difficulty

Easy

## Description

A space agency is analyzing the brightness measurements of a series of celestial events to plan future observations. For each event, they want to identify the brightness value of the nearest future event that had a strictly higher brightness. This helps them understand luminosity trends or pinpoint particularly spectacular phenomena. If no future event had higher brightness (either because it was the last event or all subsequent events had lower or equal brightness), this should be noted. Can you calculate this for each event?

## Examples

### 1

#### Input

8
[500, 400, 600, 300, 700, 450, 800, 500]

#### Output

[600, 600, 700, 700, 800, 800, -1, -1]

#### Explanation

Event 0 (500): Next higher is 600 (Event 2). Output 600.
Event 1 (400): Next higher is 600 (Event 2). Output 600.
Event 2 (600): Next higher is 700 (Event 4). Output 700.
Event 3 (300): Next higher is 700 (Event 4). Output 700.
Event 4 (700): Next higher is 800 (Event 6). Output 800.
Event 5 (450): Next higher is 800 (Event 6). Output 800.
Event 6 (800): No future event is higher. Output -1.
Event 7 (500): No future event exists. Output -1.

### 2

#### Input

5
50 50 50 50 50

#### Output

[-1, -1, -1, -1, -1]

#### Explanation

All brightness measurements are equal, so no future event has higher brightness.

## Input Format

The first line contains a single integer n, the number of events.
The second line contains n space-separated integers a_0, a_1, ..., a_[n-1], representing the brightness measurement for each event.

## Output Format

Return array of integers. The i-th integer should be the brightness of the nearest event j > i such that a_j > a_i. If no such day exists, then -1.

## Constraints

1 ≤ n ≤ 10^5
1 ≤ a_i ≤ 10^9 for all 0 ≤ i < n.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

stack, array