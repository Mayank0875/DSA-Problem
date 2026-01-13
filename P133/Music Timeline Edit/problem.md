## Title
Music Timeline Edit

## Slug
music-timeline-edit

## Difficulty
Medium

## Description
A multi-track audio project has clips. You want to splice all tracks at a point that cuts the fewest active clips.

There is a project consisting of $n$ tracks. Each track is composed of several clips, each having a specific duration (integers). The total duration of every track is identical.

You need to insert a splice marker from the start to the end of the project that minimizes the number of clips it cuts.

If the splice marker passes exactly through the silence between two clips, it is **not** considered as cutting a clip. However, you cannot place the splice marker at the very start or the very finish of the project.

Given the 2D array `structure` containing the durations of the clips in each track, return the minimum number of clips cut.

## Examples

### 1

#### Input
6
1 2 2 1
3 1 2
1 3 2
2 4
3 1 2
1 3 1 1

#### Output
2

#### Explanation
The total duration is 6.
We can insert a splice marker at distance 4 from the start.
- Track 1: 1+2+2=5 (Cut)
- Track 2: 3+1=4 (Silence)
- Track 3: 1+3=4 (Silence)
- Track 4: 2 (Cut)
- Track 5: 3+1=4 (Silence)
- Track 6: 1+3=4 (Silence)
The splice marker cuts tracks 1 and 4. Total: 2.

### 2

#### Input
3
1
1
1

#### Output
3

#### Explanation
There are no internal silences. Any splice marker drawn must cut all 3 clips.

## Input Format
- The first line contains an integer $n$, the number of tracks.
- The next $n$ lines each contain space-separated integers representing the durations of the clips in that track.

## Output Format
- Return a single integer representing the minimum number of clips cut.

## Constraints
- 1 ≤ n ≤ 10^4
- 1 <= structure[i].length <= 10^4
- The sum of elements in each row is the same.
- 1 <= structure[i][j] <= 2^31 - 1

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, hash-table, prefix-sum

