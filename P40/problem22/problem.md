## Title

Next Stronger Storm in the Infinite Loopstorm

## Slug

next-stronger-storm

## Difficulty

Easy

## Description

A meteorological team is analyzing the intensity of storms in the legendary Infinite Loopstorm sequence to forecast future weather patterns. For each storm, they want to identify the intensity of the nearest future storm that had a strictly higher intensity. This helps them understand how the storm cycle escalates or spot particularly powerful events. If no future storm had higher intensity (either because it was the last storm or all subsequent storms had lower or equal intensity), this should be noted. Can you calculate this for each storm?

## Examples

### 1

#### Input

8
[500, 400, 600, 300, 700, 450, 800, 500]

#### Output

[600, 600, 700, 700, 800, 800, -1, -1]

#### Explanation

Storm 0 (500): Next higher is 600 (Storm 2). Output 600.
Storm 1 (400): Next higher is 600 (Storm 2). Output 600.
Storm 2 (600): Next higher is 700 (Storm 4). Output 700.
Storm 3 (300): Next higher is 700 (Storm 4). Output 700.
Storm 4 (700): Next higher is 800 (Storm 6). Output 800.
Storm 5 (450): Next higher is 800 (Storm 6). Output 800.
Storm 6 (800): No future storm is higher. Output -1.
Storm 7 (500): No future storm exists. Output -1.

### 2

#### Input

5
50 50 50 50 50

#### Output

[-1, -1, -1, -1, -1]

#### Explanation

All intensities are equal, so no future storm has higher intensity.

## Input Format

The first line contains a single integer n, the number of storms.
The second line contains n space-separated integers a_0, a_1, ..., a_[n-1], representing the intensity of each storm.

## Output Format

Return array of integers. The i-th integer should be the intensity of the nearest storm j > i such that a_j > a_i. If no such day exists, then -1.

## Constraints

1 ≤ n ≤ 10^5
1 ≤ a_i ≤ 10^9 for all 0 ≤ i < n.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

stack, array