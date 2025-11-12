## Title

Previous Higher Entropy State

## Slug

previous-higher-entropy-state

## Difficulty

Easy

## Description

Imagine observing a sequence of thermodynamic states of a system, each characterized by its entropy value. As you examine each state in order, you look back (to earlier times) and want to know the entropy of the nearest previous state that has a strictly higher entropy than the current one. If all earlier states have lower or equal entropy, or if it is the first state, there is no such higher‑entropy state to the left. Your goal is to determine this higher entropy value for each position in the sequence.

## Examples

### 1

#### Input

8
[30, 60, 90, 50, 80, 40, 70, 50]

#### Output

[-1, -1, -1, 90, 90, 80, 80, 70]

#### Explanation

State 0 (30): No previous state. Output -1.
State 1 (60): State 0 (30) is lower. Output -1.
State 2 (90): States 0 (30), 1 (60) are lower. Output -1.
State 3 (50): State 2 (90) is the nearest higher. Output 90.
State 4 (80): State 2 (90) is the nearest higher. Output 90.
State 5 (40): State 4 (80) is the nearest higher. Output 80.
State 6 (70): State 4 (80) is the nearest higher. Output 80.
State 7 (50): State 6 (70) is the nearest higher. Output 70.

### 2

#### Input

5
50 50 50 50 50

#### Output

[-1, -1, -1, -1, -1]

#### Explanation

All states have equal entropy, so no strictly higher previous state exists.

## Input Format

The first line contains a single integer n, the number of states.
The second line contains n space-separated integers h_0, h_1, ..., h_[n-1], representing the entropy of each state.

## Output Format

Return array of integers. The i-th integer should be the entropy of the nearest state j < i such that h_j > h_i. If no such day exists, then -1.

## Constraints

1 ≤ n ≤ 10^5
1 ≤ h_i ≤ 10^9 for all 0 ≤ i < n.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

stack, array