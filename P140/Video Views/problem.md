## Title
Video Views

## Slug
video-views

## Difficulty
Easy

## Description
A creator checks which videos are trending based on view count.

The dashboard records the view count of $N$ videos in an array. To analyze trends, the creator needs to assign a rank to every video based on its view count.

The ranking rules are simple: the video with the **smallest** view count gets **Rank 1**. The next distinct view count gets **Rank 2**, and so on.

If two or more videos have the exact same view count, they must receive the **same rank**. The ranks must be integers starting from 1.

Your task is to replace each video's view count with its corresponding rank.

## Examples

### 1

#### Input
4
40 10 20 30

#### Output
4 1 2 3

#### Explanation
10 is the smallest (Rank 1). 20 is the second smallest (Rank 2). 30 is third (Rank 3). 40 is largest (Rank 4).

### 2

#### Input
3
2 2 2

#### Output
1 1 1

#### Explanation
All videos share the same view count, so they share Rank 1.

## Input Format
- The first line contains an integer `n`, the number of videos.
- The second line contains `n` space-separated integers representing the view counts.

## Output Format
- Return an array of integers where each element is the rank of the corresponding video.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ values ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, hash-table, sorting
