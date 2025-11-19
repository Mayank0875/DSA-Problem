## Title

Phantom Recursion

## Slug

phantom-recursion

## Difficulty

Easy

## Description

A mysterious recursive function is invoked multiple times, each invocation producing a numeric “energy” value. For each invocation, the programmer wants to identify the energy of the nearest future invocation that yields a strictly higher energy. This helps understand the growth pattern of the recursion’s power or spot particularly strong calls. If no future invocation has higher energy (either because it is the last call or all subsequent calls have lower or equal energy), this should be noted. Can you calculate this for each invocation?

## Examples

### 1

#### Input

8
[500, 400, 600, 300, 700, 450, 800, 500]

#### Output

[600, 600, 700, 700, 800, 800, -1, -1]

#### Explanation

Invocation 0 (500): Next higher is 600 (Invocation 2). Output 600.
Invocation 1 (400): Next higher is 600 (Invocation 2). Output 600.
Invocation 2 (600): Next higher is 700 (Invocation 4). Output 700.
Invocation 3 (300): Next higher is 700 (Invocation 4). Output 700.
Invocation 4 (700): Next higher is 800 (Invocation 6). Output 800.
Invocation 5 (450): Next higher is 800 (Invocation 6). Output 800.
Invocation 6 (800): No future invocation is higher. Output -1.
Invocation 7 (500): No future invocation exists. Output -1.

### 2

#### Input

5
50 50 50 50 50

#### Output

[-1, -1, -1, -1, -1]

#### Explanation

All energy values are equal, so no future invocation has higher energy.

## Input Format

The first line contains a single integer n, the number of invocations.
The second line contains n space-separated integers a_0, a_1, ..., a_[n-1], representing the energy produced by each invocation.

## Output Format

Return array of integers. The i-th integer should be the energy of the nearest invocation j > i such that a_j > a_i. If no such call exists, then -1.

## Constraints

1 ≤ n ≤ 10^5
1 ≤ a_i ≤ 10^9 for all 0 ≤ i < n.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

stack, array