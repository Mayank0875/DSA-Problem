## Title
Movie Streaming

## Slug
movie-streaming

## Difficulty
Medium

## Description
A user watches a film. 1 is HD, 0 is Pixelated. The bandwidth booster can fix k pixelated segments.

You stream a movie represented by an array `nums` consisting of 1s (HD segments) and 0s (pixelated segments), and an integer `k`. You are allowed to boost at most `k` pixelated segmentss from the sequence.

Your task is to find the length of the longest contiguous sequence of HD segmentss after performing the boosts. If the sequence contains no HD segmentss even after optimal boosts, return 0.

## Examples

### 1

#### Input
4
1 1 0 1
1

#### Output
3

#### Explanation
After boosting the element at position 2 (value 0), the sequence becomes `[1, 1, 1]`. The longest segment of HD segmentss has length 3.

### 2

#### Input
9
0 1 1 1 0 1 1 0 1
2

#### Output
6

#### Explanation
We can boost the pixelated segments at index 4 and the pixelated segments at index 7. The resulting segments of HD segmentss merge to form a sequence of length 6.

## Input Format
- The first line contains an integer `n`, representing the size of the array.
- The second line contains `n` space-separated integers representing the array `nums` (1 for HD segments, 0 for pixelated segments).
- The third line contains an integer `k`.

## Output Format
- Return a single integer representing the maximum size of the subarray of HD segmentss.

## Constraints
- 1 ≤ n ≤ 10^5
- 0 ≤ nums[i] ≤ 1
- 0 ≤ k ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
sliding-window, two-pointers, array

## Company
facebook
