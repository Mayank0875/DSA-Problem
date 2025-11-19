## Title

Shattered Spectrum

## Slug

shattered-spectrum

## Difficulty

Easy

## Description

Imagine a line of crystal shards from a shattered spectrum, each glowing with a certain intensity. As you examine each shard from left to right, you look back (to your left) and want to know the intensity of the nearest shard that shines strictly brighter than the one you are currently observing. If all previous shards are dimmer or of equal intensity, or if it's the first shard, there is no such brighter shard to the left. Your goal is to determine this brighter shard's intensity for each position along the line.

## Examples

### 1

#### Input

8
[30, 60, 90, 50, 80, 40, 70, 50]

#### Output

[-1, -1, -1, 90, 90, 80, 80, 70]

#### Explanation

Shard 0 (30): No previous shard. Output -1.
Shard 1 (60): Shard 0 (30) is dimmer. Output -1.
Shard 2 (90): Shards 0 (30), 1 (60) are dimmer. Output -1.
Shard 3 (50): Shard 2 (90) is the nearest brighter. Output 90.
Shard 4 (80): Shard 2 (90) is the nearest brighter. Output 90.
Shard 5 (40): Shard 4 (80) is the nearest brighter. Output 80.
Shard 6 (70): Shard 4 (80) is the nearest brighter. Output 80.
Shard 7 (50): Shard 6 (70) is the nearest brighter. Output 70.

### 2

#### Input

5
50 50 50 50 50

#### Output

[-1, -1, -1, -1, -1]

#### Explanation

All shards have equal intensity, so no strictly brighter previous shard exists.

## Input Format

The first line contains a single integer n, the number of shards.
The second line contains n space-separated integers h_0, h_1, ..., h_[n-1], representing the intensity of each shard.

## Output Format

Return array of integers. The i-th integer should be the intensity of the nearest shard j < i such that h_j > h_i. If no such day exists, then -1.

## Constraints

1 ≤ n ≤ 10^5
1 ≤ h_i ≤ 10^9 for all 0 ≤ i < n.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

stack, array