## Title

Spy's Shifted Codebook

## Slug

spys-shifted-codebook

## Difficulty

Medium

## Description

A spy uses a codebook where pages are numbered sequentially. To add security, the spy's personal copy is "shifted," like a rotated sorted array (e.g., [1, 2, 3, 4] becomes [3, 4, 1, 2]). You are given the shifted list of unique page numbers and a target page to find. You must find its index in O(log n) time. If the page is missing from the codebook, return -1.

## Examples

### 1

#### Input

7 0 
[4, 5, 6, 7, 0, 1, 2]


#### Output

4

#### Explanation

The key numbered 0 is at position 4 on the spun key ring.

### 2

#### Input

7 3 
[4, 5, 6, 7, 0, 1, 2]

#### Output

-1

#### Explanation

The key numbered 3 is not on this key ring.

## Input Format

- The first line contains an integers n and target , the number of keys on the ring and the number of the key to find.
- The second line contains n space-separated integers representing the key numbers after the ring was spun. All numbers are unique.

## Output Format

- Return the index (0-based position) of the target key if it exists else -1 if the target key is not found.

## Constraints

- 1 ≤ n ≤ 10^5
- 1 ≤ key_number, target ≤ 10^9
- The array is a rotation of a sorted array.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

binary-search, array