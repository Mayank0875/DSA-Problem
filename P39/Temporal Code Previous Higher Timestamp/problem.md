## Title

Temporal Code: Previous Higher Timestamp

## Slug

temporal-code-previous-higher-timestamp

## Difficulty

Easy

## Description

Imagine a sequence of code snapshots recorded over time, each associated with a timestamp representing its execution speed. As you examine each snapshot, you look back (to earlier snapshots) and want to know the timestamp of the nearest previous snapshot that is **strictly greater** than the current one. If all earlier snapshots have timestamps that are smaller or equal, or if it is the first snapshot, there is no such earlier snapshot. Your task is to determine this greater timestamp for every position in the sequence.

## Examples

### 1

#### Input

8
[30, 60, 90, 50, 80, 40, 70, 50]

#### Output

[-1, -1, -1, 90, 90, 80, 80, 70]

#### Explanation

Snapshot 0 (30): No previous snapshot. Output -1.  
Snapshot 1 (60): Snapshot 0 (30) is smaller. Output -1.  
Snapshot 2 (90): Snapshots 0 (30), 1 (60) are smaller. Output -1.  
Snapshot 3 (50): Snapshot 2 (90) is the nearest greater. Output 90.  
Snapshot 4 (80): Snapshot 2 (90) is the nearest greater. Output 90.  
Snapshot 5 (40): Snapshot 4 (80) is the nearest greater. Output 80.  
Snapshot 6 (70): Snapshot 4 (80) is the nearest greater. Output 80.  
Snapshot 7 (50): Snapshot 6 (70) is the nearest greater. Output 70.

### 2

#### Input

5
50 50 50 50 50

#### Output

[-1, -1, -1, -1, -1]

#### Explanation

All snapshots have equal timestamps, so no strictly greater previous snapshot exists.

## Input Format

The first line contains a single integer n, the number of snapshots.  
The second line contains n space-separated integers h_0, h_1, ..., h_[n-1], representing the timestamp of each snapshot.

## Output Format

Return array of integers. The i-th integer should be the timestamp of the nearest snapshot j < i such that h_j > h_i. If no such snapshot exists, then -1.

## Constraints

1 ≤ n ≤ 10^5  
1 ≤ h_i ≤ 10^9 for all 0 ≤ i < n.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

stack, array