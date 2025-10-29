## Title

Double Xor

## Slug

double-xor

## Difficulty

Easy

## Description

You are given an array A₁, A₂, A₃, …, Aₙ consisting of integers and an integer K representing the window size.
Your task is to slide a window of size K across the array from left to right and, for each window, calculate the XOR of all elements inside it.

After finding the XOR for each window, calculate the XOR of all these window XORs and output the final result.

## Examples

### 1

#### Input

5 3
[1, 2, 3, 4, 5]

#### Output

7

#### Explanation

All windows of size 3 are:
	•	[1, 2, 3] → XOR = 0
	•	[2, 3, 4] → XOR = 5
	•	[3, 4, 5] → XOR = 2

Final XOR = 0 ^ 5 ^ 2 = 7

### 2

#### Input

4 2
[5, 1, 3, 2]

#### Output

7

#### Explanation

Windows:
	•	[5, 1] → XOR = 4
	•	[1, 3] → XOR = 2
	•	[3, 2] → XOR = 1

Final XOR = 4 ^ 2 ^ 1 = 7

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

arrays, sliding window
