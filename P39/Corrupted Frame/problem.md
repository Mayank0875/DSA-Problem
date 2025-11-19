## Title

Corrupted Frame

## Slug

corrupted-frame

## Difficulty

Easy

## Description

Imagine analyzing a sequence of video frames, each with a certain level of corruption measured as an integer. As you examine each frame, you look back at the earlier frames (to its left) and want to know the corruption level of the nearest previous frame that is strictly more corrupted than the current one. If all earlier frames have lower or equal corruption, or if it is the first frame, there is no such more corrupted frame to the left. Your goal is to determine this higher corruption level for each position in the sequence.

## Examples

### 1

#### Input

8
[30, 60, 90, 50, 80, 40, 70, 50]

#### Output

[-1, -1, -1, 90, 90, 80, 80, 70]

#### Explanation

Frame 0 (30): No previous frame. Output -1.
Frame 1 (60): Frame 0 (30) is less corrupted. Output -1.
Frame 2 (90): Frames 0 (30), 1 (60) are less corrupted. Output -1.
Frame 3 (50): Frame 2 (90) is the nearest more corrupted. Output 90.
Frame 4 (80): Frame 2 (90) is the nearest more corrupted. Output 90.
Frame 5 (40): Frame 4 (80) is the nearest more corrupted. Output 80.
Frame 6 (70): Frame 4 (80) is the nearest more corrupted. Output 80.
Frame 7 (50): Frame 6 (70) is the nearest more corrupted. Output 70.

### 2

#### Input

5
50 50 50 50 50

#### Output

[-1, -1, -1, -1, -1]

#### Explanation

All frames have equal corruption, so no strictly more corrupted previous frame exists.

## Input Format

The first line contains a single integer n, the number of frames.
The second line contains n space-separated integers h_0, h_1, ..., h_[n-1], representing the corruption level of each frame.

## Output Format

Return array of integers. The i-th integer should be the corruption level of the nearest frame j < i such that h_j > h_i. If no such frame exists, then -1.

## Constraints

1 ≤ n ≤ 10^5
1 ≤ h_i ≤ 10^9 for all 0 ≤ i < n.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

stack, array