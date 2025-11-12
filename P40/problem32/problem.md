## Title

The Vanishing Loop

## Slug

the-vanishing-loop

## Difficulty

Easy

## Description

A programmer is investigating a mysterious loop that seems to vanish after certain iterations. For each iteration, they want to know the value of the nearest future iteration where the loop variable becomes **strictly larger** than its current value. This helps them understand the loop’s growth pattern before it disappears. If no such future iteration exists (either because it is the last iteration or all subsequent values are lower or equal), this should be noted. Can you determine this for every iteration?

## Examples

### 1

#### Input

8
[500, 400, 600, 300, 700, 450, 800, 500]

#### Output

[600, 600, 700, 700, 800, 800, -1, -1]

#### Explanation

Iteration 0 (500): Next higher is 600 (Iteration 2). Output 600.  
Iteration 1 (400): Next higher is 600 (Iteration 2). Output 600.  
Iteration 2 (600): Next higher is 700 (Iteration 4). Output 700.  
Iteration 3 (300): Next higher is 700 (Iteration 4). Output 700.  
Iteration 4 (700): Next higher is 800 (Iteration 6). Output 800.  
Iteration 5 (450): Next higher is 800 (Iteration 6). Output 800.  
Iteration 6 (800): No future iteration is higher. Output -1.  
Iteration 7 (500): No future iteration exists. Output -1.

### 2

#### Input

5
50 50 50 50 50

#### Output

[-1, -1, -1, -1, -1]

#### Explanation

All values are equal, so no future iteration has a higher value.

## Input Format

The first line contains a single integer n, the number of iterations.  
The second line contains n space-separated integers a_0, a_1, ..., a_[n-1], representing the loop variable’s value at each iteration.

## Output Format

Return array of integers. The i-th integer should be the value of the nearest iteration j > i such that a_j > a_i. If no such iteration exists, then -1.

## Constraints

1 ≤ n ≤ 10^5  
1 ≤ a_i ≤ 10^9 for all 0 ≤ i < n.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

stack, array