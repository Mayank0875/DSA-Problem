## Title

Binary Bloom: Next Higher Intensity

## Slug

binary-bloom-next-higher-intensity

## Difficulty

Easy

## Description

A garden of binary blossoms records the intensity of each bloom over time. For each recorded intensity, the horticulturists want to find the intensity of the nearest future bloom that is strictly higher. This helps them understand growth patterns and identify standout blossoms. If no future bloom has a higher intensity (either because it is the last record or all subsequent intensities are lower or equal), this should be noted. Can you calculate this for each recorded intensity?

## Examples

### 1

#### Input

8
[500, 400, 600, 300, 700, 450, 800, 500]

#### Output

[600, 600, 700, 700, 800, 800, -1, -1]

#### Explanation

Bloom 0 (500): Next higher is 600 (Bloom 2). Output 600.
Bloom 1 (400): Next higher is 600 (Bloom 2). Output 600.
Bloom 2 (600): Next higher is 700 (Bloom 4). Output 700.
Bloom 3 (300): Next higher is 700 (Bloom 4). Output 700.
Bloom 4 (700): Next higher is 800 (Bloom 6). Output 800.
Bloom 5 (450): Next higher is 800 (Bloom 6). Output 800.
Bloom 6 (800): No future bloom is higher. Output -1.
Bloom 7 (500): No future bloom exists. Output -1.

### 2

#### Input

5
50 50 50 50 50

#### Output

[-1, -1, -1, -1, -1]

#### Explanation

All intensities are equal, so no future bloom has higher intensity.

## Input Format

The first line contains a single integer n, the number of recorded intensities.
The second line contains n space-separated integers a_0, a_1, ..., a_[n-1], representing the intensity of each binary bloom.

## Output Format

Return array of integers. The i-th integer should be the intensity of the nearest bloom j > i such that a_j > a_i. If no such day exists, then -1.

## Constraints

1 ≤ n ≤ 10^5
1 ≤ a_i ≤ 10^9 for all 0 ≤ i < n.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

stack, array