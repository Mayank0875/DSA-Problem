## Title
Digital Photo Album

## Slug
digital-photo-album

## Difficulty
Hard

## Description
You have `n` photos to upload to `k` folders. Photos have file sizes and differ in resolution. The 'upload latency' for a folder is the square of the total size of photos inside.

You must partition the sequence of photos into exactly `k` non-empty contiguous folders.
Each folder corresponds to a folder.
The "upload latency" for a folder is calculated as the **square of the sum** of the sizes of the photos in that folder.

Your goal is to minimize the total upload latency (the sum of the upload latency values of all `k` folders).

## Examples

### 1

#### Input
8 3
2 3 1 2 2 3 4 1

#### Output
110

#### Explanation
We partition the photos into 3 folders: `[2, 3, 1]`, `[2, 2, 3]`, and `[4, 1]`.
The sums are 6, 7, 5.
The total upload latency is $6^2 + 7^2 + 5^2 = 36 + 49 + 25 = 110$.

### 2

#### Input
5 1
1 2 3 4 5

#### Output
225

#### Explanation
Only 1 folder is allowed, containing all photos. Sum = 15. upload latency = $15^2 = 225$.

## Input Format
- The first line contains two integers `n` and `k`: the number of photos and the required number of folders.
- The second line contains `n` integers representing the sizes of each photo.

## Output Format
- Return one integer: the minimum total upload latency.

## Constraints
- 1 ≤ k ≤ n ≤ 3000
- 1 ≤ value ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, array
