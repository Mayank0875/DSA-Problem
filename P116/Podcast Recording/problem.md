## Title
Podcast Recording

## Slug
podcast-recording

## Difficulty
Medium

## Description
A studio records episodes. Each episode books the room from start to end.

The calendar shows list of episodes, each defined by a start and an end, represented as a pair `[s, e]`.

The room must be reset. An episode must end strictly before the next one starts. Specifically, to transition from episode `[a, b]` to a subsequent episode `[c, d]`, the e of the first episode must be **strictly less than** the s of the second episode (i.e., `b < c`).

You can select episodes in any order you like to form a valid recording day. Your goal is to determine the maximum number of episodes that can be included in a single recording day.

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
The longest recording day is `[1, 2] -> [3, 4]`. You cannot include `[2, 3]` because `2` (end of first) is not strictly less than `2` (start of second).

### 2

#### Input
3
1 2
7 8
4 5

#### Output
3

#### Explanation
The episodes can be reordered to form the recording day `[1, 2] -> [4, 5] -> [7, 8]`. All transitions satisfy `end < start`.

## Input Format
- The first line contains an integer `n`, the number of available episodes.
- The next `n` lines each contain two integers, representing the `s` and `e` of an episode.

## Output Format
- Return a single integer representing the maximum length of the recording day.

## Constraints
- 1 ≤ n ≤ 1000
- -1000 ≤ s < e ≤ 1000

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, dynamic-programming, greedy, sorting
