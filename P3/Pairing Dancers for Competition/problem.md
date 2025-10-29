## Title

Pairing Dancers for Competition

## Slug

pairing-dancers-competition

## Difficulty

Easy

## Description

A dance competition organizer needs to form pairs of dancers. Some dancers might perform solo. Each pair (or solo dancer) is judged, and their 'complexity score' (represented by weight) contributes to the overall performance slot. A performance slot has a maximum complexity score limit of `x`. A slot can accommodate either one solo dancer or a pair of dancers. Given the complexity scores of `n` dancers, find the minimum number of performance slots needed to include all dancers without exceeding the complexity limit per slot.

## Examples

### 1

#### Input

4 10
[7, 2, 3, 9]

#### Output

3

#### Explanation

One optimal scheduling:
    - Slot 1: Dancer with score 2 and dancer with score 7 (Total score 9 <= 10)
    - Slot 2: Dancer with score 3 (Total score 3 <= 10)
    - Slot 3: Dancer with score 9 (Total score 9 <= 10)
This requires 3 slots.

### 2

#### Input

5 5
[2, 2, 2, 3, 4]

#### Output

3

#### Explanation

One optimal scheduling:
    - Slot 1: Dancer with score 2 and dancer with score 3 (Total score 5 <= 5)
    - Slot 2: Two dancers with score 2 (Total score 4 <= 5)
    - Slot 3: Dancer with score 4 (Total score 4 <= 5)
This requires 3 slots.

## Input Format

- The first line contains two integers n and x: the number of dancers and the maximum complexity score per slot.
- The second line contains n integers p_1, p_2, ..., p_n: the complexity score of each dancer.

## Output Format

- Return a single integer: the minimum number of performance slots required.

## Constraints

- 1 ≤ n ≤ 1e5
- 1 ≤ x ≤ 1e9
- 1 ≤ p_i ≤ x

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

greedy, sorting, two pointers