## Title
Playlist CD Burning

## Slug
playlist-cd-burning

## Difficulty
Hard

## Description
You want to burn `n` songs onto `k` CDs. Songs have file sizes. They must stay in playlist order. The 'spin imbalance' of a CD is the square of the total size of songs on it.

You must partition the sequence of songs into exactly `k` non-empty contiguous discs.
Each disc corresponds to a CD.
The "spin imbalance" for a CD is calculated as the **square of the sum** of the file sizes of the songs in that disc.

Your goal is to minimize the total spin imbalance (the sum of the spin imbalance values of all `k` discs).

## Examples

### 1

#### Input
8 3
2 3 1 2 2 3 4 1

#### Output
110

#### Explanation
We partition the songs into 3 discs: `[2, 3, 1]`, `[2, 2, 3]`, and `[4, 1]`.
The sums are 6, 7, 5.
The total spin imbalance is $6^2 + 7^2 + 5^2 = 36 + 49 + 25 = 110$.

### 2

#### Input
5 1
1 2 3 4 5

#### Output
225

#### Explanation
Only 1 disc is allowed, containing all songs. Sum = 15. spin imbalance = $15^2 = 225$.

## Input Format
- The first line contains two integers `n` and `k`: the number of songs and the required number of discs.
- The second line contains `n` integers representing the file sizes of each song.

## Output Format
- Return one integer: the minimum total spin imbalance.

## Constraints
- 1 ≤ k ≤ n ≤ 3000
- 1 ≤ value ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, array
