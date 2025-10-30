## Title

Robot's Energy

## Slug

robots-energy

## Difficulty

Medium

## Description

A small robot moves along a linear track with N positions, from 1 to N. At each position `i`, the robot can absorb `A[i]` units of energy, where `A[i]` is an integer from 0 to 9.
A "successful segment" of the track, from position L to R (inclusive), is defined as a segment where the total energy absorbed (`A[L] + ... + A[R]`) is exactly equal to the number of positions in that segment (R - L + 1).
Your task is to find the total number of successful segments on the track.

Note: The array is 1-based indexed, i.e., the first element is A₁.

## Examples

### 1

#### Input

5
[1, 1, 0, 1, 1]

#### Output

6

#### Explanation

There are 6 successful segments: A[1 .. 1], A[2 .. 2], A[1 .. 2], A[4 .. 4], A[5 .. 5], A[4 .. 5]

### 2

#### Input

3
[1, 2, 0]

#### Output

3

#### Explanation

There are 3 successful segments: A[1 .. 1], A[2 .. 3], A[1 .. 3]

## Input Format

- The first line contains an integer N, the size of the array. 
- The second line contains N space-separated integers, representing the elements of the array (0 to 9).

## Output Format

- Return a single integer, the number of successful segments.

## Constraints

- 1 ≤ N ≤ 10^5
- 0 ≤ arr[i] ≤ 9

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

arrays, prefix sum, hash map