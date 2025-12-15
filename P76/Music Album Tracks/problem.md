## Title
Music Album Tracks

## Slug
music-album-tracks

## Difficulty
Hard

## Description
A musician groups `n` recorded tracks into `k` sides of vinyl records. Each track has a duration. Tracks must remain in order. The 'groove distortion' of a side is the square of its total duration.

You must partition the sequence of tracks into exactly `k` non-empty contiguous sides.
Each side corresponds to a vinyl side.
The "groove distortion" for a vinyl side is calculated as the **square of the sum** of the durations of the tracks in that side.

Your goal is to minimize the total groove distortion (the sum of the groove distortion values of all `k` sides).

## Examples

### 1

#### Input
8 3
2 3 1 2 2 3 4 1

#### Output
110

#### Explanation
We partition the tracks into 3 sides: `[2, 3, 1]`, `[2, 2, 3]`, and `[4, 1]`.
The sums are 6, 7, 5.
The total groove distortion is $6^2 + 7^2 + 5^2 = 36 + 49 + 25 = 110$.

### 2

#### Input
5 1
1 2 3 4 5

#### Output
225

#### Explanation
Only 1 side is allowed, containing all tracks. Sum = 15. groove distortion = $15^2 = 225$.

## Input Format
- The first line contains two integers `n` and `k`: the number of tracks and the required number of sides.
- The second line contains `n` integers representing the durations of each track.

## Output Format
- Return one integer: the minimum total groove distortion.

## Constraints
- 1 ≤ k ≤ n ≤ 3000
- 1 ≤ value ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, array
