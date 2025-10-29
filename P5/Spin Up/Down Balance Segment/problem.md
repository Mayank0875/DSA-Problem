## Title

Spin Up/Down Balance Segment

## Slug

spin-up-down-balance-segment

## Difficulty

Easy

## Description

In a physics experiment, the spin states of a sequence of particles are measured, recorded as '0' for spin down and '1' for spin up. Researchers are looking for the longest continuous segment of particles where the number of spin-up particles equals the number of spin-down particles. This might indicate a region of specific interaction or neutrality. Given the sequence of spin states, find the length of the longest such balanced segment.

## Examples

### 1

#### Input

2
[0, 1]

#### Output

2

#### Explanation

The segment [0, 1] (Spin Down, Spin Up) is the longest balanced segment.

### 2

#### Input

3
[0, 1, 0]

#### Output

2

#### Explanation

[0, 1] and [1, 0] are the longest balanced segments.

## Input Format

- The first line contains a single integer N, the number of particles measured.
- The second line contains N space-separated integers, representing the spin states (0 for down, 1 for up).

## Output Format

- Return a single integer representing the length of the longest contiguous balanced spin segment.

## Constraints

- 1 ≤ N ≤ 10^5
- 0 ≤ arr[i] ≤ 1

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

arrays, physics, prefix sum, hashmap