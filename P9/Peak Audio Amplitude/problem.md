## Title

Peak Audio Amplitude

## Slug

peak-audio-amplitude

## Difficulty

Medium

## Description

You are analyzing a digital audio signal represented by N samples in array A. You need to process the audio in chunks of size K (a sliding window). For each chunk, you must find the *peak amplitude* (the MAX sample value). After analyzing the entire signal, you must compute the XOR sum of all the peak amplitudes.

## Examples

### 1

#### Input

5 3
[1, 2, 3, 4, 5]

#### Output

2

#### Explanation

All windows of size 3 are:
    •   [1, 2, 3] → MAX = 3
    •   [2, 3, 4] → MAX = 4
    •   [3, 4, 5] → MAX = 5

Final XOR = 3 ^ 4 ^ 5 = 2

### 2

#### Input

4 2
[5, 1, 3, 2]

#### Output

5

#### Explanation

Windows:
    •   [5, 1] → MAX = 5
    •   [1, 3] → MAX = 3
    •   [3, 2] → MAX = 3

Final XOR = 5 ^ 3 ^ 3 = 5

## Input Format

- The first line contains two integers N (size of array) and K (window size).
- The second line contains N space-separated integers — the elements of the array.

## Output Format

- Return a single integer — the final XOR of all window XORs.

## Constraints

- 1 ≤ N ≤ 10^5
- 1 ≤ K ≤ N
- 0 ≤ arr[i] ≤ 1e9

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

arrays, sliding window, deque