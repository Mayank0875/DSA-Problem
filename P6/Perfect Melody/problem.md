## Title

Perfect Melody

## Slug

perfect-melody

## Difficulty

Medium

## Description

A song is composed of N notes, played in sequence. Each note `i` has a "harmony value" `A[i]` (an integer from 0 to 9).
A "perfect melody" is a contiguous sequence of notes, from L to R, where the sum of the harmony values (`A[L] + ... + A[R]`) is exactly equal to the number of notes in the sequence (R - L + 1).
Please calculate the total number of perfect melodies within the song.

Note: The array is 1-based indexed, i.e., the first element is A₁.

## Examples

### 1

#### Input

5
[1, 1, 0, 1, 1]

#### Output

6

#### Explanation

There are 6 perfect melodies: A[1 .. 1], A[2 .. 2], A[1 .. 2], A[4 .. 4], A[5 .. 5], A[4 .. 5]

### 2

#### Input

3
[1, 2, 0]

#### Output

3

#### Explanation

There are 3 perfect melodies: A[1 .. 1], A[2 .. 3], A[1 .. 3]

## Input Format

- The first line contains an integer N, the size of the array. 
- The second line contains N space-separated integers, representing the elements of the array (0 to 9).

## Output Format

- Return a single integer, the number of perfect melodies.

## Constraints

- 1 ≤ N ≤ 10^5
- 0 ≤ arr[i] ≤ 9

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

arrays, prefix sum, hash map