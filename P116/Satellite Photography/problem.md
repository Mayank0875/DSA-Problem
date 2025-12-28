## Title
Satellite Photography

## Slug
satellite-photography

## Difficulty
Medium

## Description
A satellite takes photos. Each photo covers a latitude range.

Requests list list of photos, each defined by a south lat and an north lat, represented as a pair `[S, N]`.

To form a non-overlapping strip map, the north latitude of one photo must be strictly less than the south latitude of the next. Specifically, to transition from photo `[a, b]` to a subsequent photo `[c, d]`, the N of the first photo must be **strictly less than** the S of the second photo (i.e., `b < c`).

You can select photos in any order you like to form a valid mosaic. Your goal is to determine the maximum number of photos that can be included in a single mosaic.

## Examples

### 1

#### Input
3
1 2
2 3
3 4

#### Output
2

#### Explanation
The longest mosaic is `[1, 2] -> [3, 4]`. You cannot include `[2, 3]` because `2` (end of first) is not strictly less than `2` (start of second).

### 2

#### Input
3
1 2
7 8
4 5

#### Output
3

#### Explanation
The photos can be reordered to form the mosaic `[1, 2] -> [4, 5] -> [7, 8]`. All transitions satisfy `end < start`.

## Input Format
- The first line contains an integer `n`, the number of available photos.
- The next `n` lines each contain two integers, representing the `S` and `N` of an photo.

## Output Format
- Return a single integer representing the maximum length of the mosaic.

## Constraints
- 1 ≤ n ≤ 1000
- -1000 ≤ S < N ≤ 1000

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, dynamic-programming, greedy, sorting
