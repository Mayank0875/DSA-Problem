## Title

Single File in Corrupted Drive

## Slug

single-file-corrupted-drive

## Difficulty

Medium

## Description

You are recovering data from a corrupted hard drive. The files, when sorted by their ID, should all be in pairs (a file and its backup). Due to the corruption, all pairs are intact except for one file, which lost its backup. This file's ID appears only once. Find the ID of the single, un-backed-up file from the sorted list.

You must write an algorithm with O(log n) runtime complexity.

## Examples

### 1

#### Input

9 
[1, 1, 2, 3, 3, 4, 4, 8, 8]


#### Output

2

#### Explanation

In the sequence [1, 1, 2, 3, 3, 4, 4, 8, 8], the number 2 appears only once.

### 2

#### Input

7 
[3, 3, 7, 7, 10, 11, 11]

#### Output

10

#### Explanation

In the sequence [3, 3, 7, 7, 10, 11, 11], the number 10 appears only once.

## Input Format

- The first line contains an odd integer n, the total number of files.
- The second line contains n space-separated integers representing the sorted file IDs.

## Output Format

- Return a single integer: the file ID that appears only once.

## Constraints

- 1 ≤ n ≤ 10^5
- 1 ≤ stone_value ≤ 10^9
- The array is sorted.
- Every element appears twice except for one.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

binary-search, array