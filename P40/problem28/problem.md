## Title

The Obsidian Key

## Slug

the-obsidian-key

## Difficulty

Easy

## Description

A daring explorer is navigating a sequence of ancient chambers, each containing a fragment of the legendary Obsidian Key. Every fragment has a power rating, and the explorer wishes to know, for each fragment, the power rating of the nearest future fragment that possesses a strictly higher power. This information helps the explorer gauge the progression of the key’s potency and plan the optimal path forward. If no later fragment has a higher power (either because it is the last chamber or all subsequent fragments have lower or equal power), this should be noted. Can you determine this for each fragment?

## Examples

### 1

#### Input

8
[500, 400, 600, 300, 700, 450, 800, 500]

#### Output

[600, 600, 700, 700, 800, 800, -1, -1]

#### Explanation

Fragment 0 (500): Next higher is 600 (Fragment 2). Output 600.  
Fragment 1 (400): Next higher is 600 (Fragment 2). Output 600.  
Fragment 2 (600): Next higher is 700 (Fragment 4). Output 700.  
Fragment 3 (300): Next higher is 700 (Fragment 4). Output 700.  
Fragment 4 (700): Next higher is 800 (Fragment 6). Output 800.  
Fragment 5 (450): Next higher is 800 (Fragment 6). Output 800.  
Fragment 6 (800): No future fragment is higher. Output -1.  
Fragment 7 (500): No future fragment exists. Output -1.

### 2

#### Input

5
50 50 50 50 50

#### Output

[-1, -1, -1, -1, -1]

#### Explanation

All power ratings are equal, so no future fragment has higher power.

## Input Format

The first line contains a single integer n, the number of fragments.  
The second line contains n space-separated integers a_0, a_1, ..., a_[n-1], representing the power rating of each fragment.

## Output Format

Return array of integers. The i-th integer should be the power rating of the nearest fragment j > i such that a_j > a_i. If no such fragment exists, then -1.

## Constraints

1 ≤ n ≤ 10^5  
1 ≤ a_i ≤ 10^9 for all 0 ≤ i < n.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

stack, array