## Title

Rotated Musical Scale

## Slug

rotated-musical-scale

## Difficulty

Medium

## Description

A musical scale is represented by unique note frequency numbers, sorted in ascending order. A musician starts playing the scale from a random note, creating a "rotated" sorted sequence (e.g., [261, 293, 329, 349] might become [329, 349, 261, 293]). You are given this rotated list. Your task is to find the base note of the scale, which is the one with the minimum frequency. Find this minimum value in O(log n) time.

## Examples

### 1

#### Input

7
[4, 5, 6, 7, 0, 1, 2]

#### Output

0

#### Explanation

The smallest value in this rotated sequence is 0.

### 2

#### Input

6
[4, 5, 6, 7, 1, 2]

#### Output

1

#### Explanation

The smallest value in this rotated sequence is 1.

## Input Format

- The first line contains an integer n, the number of items.
- The second line contains n space-separated integers representing the item numbers after rotation. All numbers are unique.

## Output Format

- Return a single integer representing the minimum item number found.

## Constraints

- 1 ≤ n ≤ 10^5
- 1 ≤ gem_number ≤ 10^9
- The array is guaranteed to be a rotation of a sorted array.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

binary-search, array