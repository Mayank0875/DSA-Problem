## Title
Bridge Construction

## Slug
bridge-construction

## Difficulty
Medium

## Description
Engineers are building a pontoon bridge using specific segments. Each segment spans from a start coordinate to an end coordinate.

There is a list of segments, each defined by a start pos and an end pos, represented as a pair `[s, e]`.

Segments must not overlap physically. To place a segment after another, the end of the previous segment must be strictly less than the start of the next (leaving a safety gap). Specifically, to transition from segment `[a, b]` to a subsequent segment `[c, d]`, the e of the first segment must be **strictly less than** the s of the second segment (i.e., `b < c`).

You can select segments in any order you like to form a valid bridge. Your goal is to determine the maximum number of segments that can be included in a single bridge.

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
The longest bridge is `[1, 2] -> [3, 4]`. You cannot include `[2, 3]` because `2` (end of first) is not strictly less than `2` (start of second).

### 2

#### Input
3
1 2
7 8
4 5

#### Output
3

#### Explanation
The segments can be reordered to form the bridge `[1, 2] -> [4, 5] -> [7, 8]`. All transitions satisfy `end < start`.

## Input Format
- The first line contains an integer `n`, the number of available segments.
- The next `n` lines each contain two integers, representing the `s` and `e` of an segment.

## Output Format
- Return a single integer representing the maximum length of the bridge.

## Constraints
- 1 ≤ n ≤ 1000
- -1000 ≤ s < e ≤ 1000

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, dynamic-programming, greedy, sorting
