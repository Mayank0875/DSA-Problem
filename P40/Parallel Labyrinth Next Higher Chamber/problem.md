## Title

Parallel Labyrinth: Next Higher Chamber

## Slug

parallel-labyrinth-next-higher-chamber

## Difficulty

Easy

## Description

Adventurers are exploring a series of chambers in a parallel labyrinth. Each chamber has a difficulty rating, and for every chamber they want to know the difficulty of the nearest future chamber that is strictly more challenging. This helps them decide where to prepare extra resources or identify the toughest upcoming sections. If there is no later chamber with a higher difficulty (either because it is the final chamber or all subsequent chambers are easier or equally difficult), this should be indicated. Can you determine this for each chamber?

## Examples

### 1

#### Input

8
[500, 400, 600, 300, 700, 450, 800, 500]

#### Output

[600, 600, 700, 700, 800, 800, -1, -1]

#### Explanation

Chamber 0 (500): Next higher is 600 (Chamber 2). Output 600.
Chamber 1 (400): Next higher is 600 (Chamber 2). Output 600.
Chamber 2 (600): Next higher is 700 (Chamber 4). Output 700.
Chamber 3 (300): Next higher is 700 (Chamber 4). Output 700.
Chamber 4 (700): Next higher is 800 (Chamber 6). Output 800.
Chamber 5 (450): Next higher is 800 (Chamber 6). Output 800.
Chamber 6 (800): No future chamber is higher. Output -1.
Chamber 7 (500): No future chamber exists. Output -1.

### 2

#### Input

5
50 50 50 50 50

#### Output

[-1, -1, -1, -1, -1]

#### Explanation

All difficulties are equal, so no future chamber has higher difficulty.

## Input Format

The first line contains a single integer n, the number of chambers.
The second line contains n space-separated integers a_0, a_1, ..., a_[n-1], representing the difficulty rating for each chamber.

## Output Format

Return array of integers. The i-th integer should be the difficulty of the nearest chamber j > i such that a_j > a_i. If no such chamber exists, then -1.

## Constraints

1 ≤ n ≤ 10^5
1 ≤ a_i ≤ 10^9 for all 0 ≤ i < n.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

stack, array