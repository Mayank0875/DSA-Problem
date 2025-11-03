## Title

Corrupted File System

## Slug

corrupted-file-system

## Difficulty

Medium

## Description

A data recovery specialist is trying to restore a directory. The files, identified by unique numbers, were originally sorted. A data corruption event has "rotated" this sorted list (e.g., [10, 20, 30] became [30, 10, 20]). To begin the repair, the specialist must find the starting point of the original sequence, which is the file with the minimum ID. Given the sequence of file IDs as they appear in the corrupted directory, find this minimum ID.

You must write an algorithm with O(log n) runtime complexity.

## Examples

### 1

#### Input

7
[4, 5, 6, 7, 0, 1, 2]

#### Output

0

#### Explanation

The smallest file ID in this rotated sequence is 0.

### 2

#### Input

6
[4, 5, 6, 7, 1, 2]

#### Output

1

#### Explanation

The smallest file ID in this rotated sequence is 1.

### 3

#### Input

5
[1, 2, 3, 4, 5]

#### Output

1

#### Explanation

The list was not rotated (or rotated 0 times). The minimum is the first element.

## Input Format

- The first line contains an integer `n`, the number of files.
- The second line contains `n` space-separated integers representing the file IDs after rotation. All numbers are unique.

## Output Format

- Return a single integer representing the minimum file ID found.

## Constraints

- 1 ≤ n ≤ 10^5
- 0 ≤ file_ID ≤ 10^9
- The array is guaranteed to be a rotation of a sorted array.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

binary-search, array