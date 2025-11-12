## Title

Corrupted Frame Restoration

## Slug

corrupted-frame-restoration

## Difficulty

Easy

## Description

A video processing system is analyzing a sequence of frames, each assigned a corruption score (higher means more corrupted). For every frame, the system wants to determine the corruption score of the nearest future frame that has a strictly lower corruption score (i.e., a cleaner frame). This helps in planning restoration steps or identifying the next viable frame for processing. If no later frame is cleaner (either because it is the last frame or all subsequent frames are equally or more corrupted), this should be noted. Can you compute this for each frame?

## Examples

### 1

#### Input

8
[500, 400, 600, 300, 700, 450, 800, 500]

#### Output

[600, 600, 700, 700, 800, 800, -1, -1]

#### Explanation

Frame 0 (500): Next cleaner is 600 (Frame 2). Output 600.
Frame 1 (400): Next cleaner is 600 (Frame 2). Output 600.
Frame 2 (600): Next cleaner is 700 (Frame 4). Output 700.
Frame 3 (300): Next cleaner is 700 (Frame 4). Output 700.
Frame 4 (700): Next cleaner is 800 (Frame 6). Output 800.
Frame 5 (450): Next cleaner is 800 (Frame 6). Output 800.
Frame 6 (800): No future frame is cleaner. Output -1.
Frame 7 (500): No future frame exists. Output -1.

### 2

#### Input

5
50 50 50 50 50

#### Output

[-1, -1, -1, -1, -1]

#### Explanation

All corruption scores are equal, so no future frame is cleaner.

## Input Format

The first line contains a single integer n, the number of frames.
The second line contains n space-separated integers a_0, a_1, ..., a_[n-1], representing the corruption score for each frame.

## Output Format

Return array of integers. The i-th integer should be the corruption score of the nearest frame j > i such that a_j > a_i. If no such frame exists, then -1.

## Constraints

1 ≤ n ≤ 10^5
1 ≤ a_i ≤ 10^9 for all 0 ≤ i < n.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

stack, array