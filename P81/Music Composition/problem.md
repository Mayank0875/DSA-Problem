## Title
Music Composition

## Slug
music-composition

## Difficulty
Medium

## Description
A melody transitions from Note 1 to Note n.

The scale has `n` notes and `m` directed intervals. Intervals may repeat between the same pair of notes and self-loops are allowed. A melody of length `k` is a sequence of exactly `k` directed intervals; notes and intervals may be visited multiple times.

Given `n`, `m`, `k` and a list of the `m` directed intervals (each interval given as two integers `u` `v` meaning a directed interval from `u` to `v`), compute the number of distinct melodies that start at note 1 and end at note `n` with length exactly `k`. Output the answer modulo 1000000007.

## Examples

### 1

#### Input
3 4 8
1 2
2 3
3 1
3 2

#### Output
2

#### Explanation
We have 3 notes. We want the number of directed melodies of length 8 from note 1 to note 3.
Valid length-8 melodies:
1 -> 2 -> 3 -> 1 -> 2 -> 3 -> 1 -> 2 -> 3
1 -> 2 -> 3 -> 2 -> 3 -> 1 -> 2 -> 3
There are 2 such melodies.

### 2

#### Input
3 4 2
1 2
2 3
3 1
3 2

#### Output
1

#### Explanation
Assuming the graph has intervals 1->2 and 2->3, the only melody of length 2 from note 1 to note 3 is:
1 -> 2 -> 3

## Input Format
- The first line contains three integers n, m, and k: the number of notes, intervals, and the required melody length.
- The next m lines describe the intervals. Each line contains two integers u and v, indicating a directed interval from note u to note v.

## Output Format
- Return single integer: the number of melodies modulo 10^9+7.

## Constraints
- 1 ≤ n ≤ 100
- 1 ≤ m ≤ 10^5
- 1 ≤ k ≤ 10^18
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph, dynamic-programming
