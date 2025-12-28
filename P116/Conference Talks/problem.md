## Title
Conference Talks

## Slug
conference-talks

## Difficulty
Medium

## Description
A researcher attends a conference with many sessions. Each session has a time slot.

The program lists list of talks, each defined by a begin time and an finish time, represented as a pair `[begin, finish]`.

You need time to walk between rooms. A talk must finish strictly before the next one begins to attend both. Specifically, to transition from talk `[a, b]` to a subsequent talk `[c, d]`, the finish of the first talk must be **strictly less than** the begin of the second talk (i.e., `b < c`).

You can select talks in any order you like to form a valid itinerary. Your goal is to determine the maximum number of talks that can be included in a single itinerary.

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
The longest itinerary is `[1, 2] -> [3, 4]`. You cannot include `[2, 3]` because `2` (end of first) is not strictly less than `2` (start of second).

### 2

#### Input
3
1 2
7 8
4 5

#### Output
3

#### Explanation
The talks can be reordered to form the itinerary `[1, 2] -> [4, 5] -> [7, 8]`. All transitions satisfy `end < start`.

## Input Format
- The first line contains an integer `n`, the number of available talks.
- The next `n` lines each contain two integers, representing the `begin` and `finish` of an talk.

## Output Format
- Return a single integer representing the maximum length of the itinerary.

## Constraints
- 1 ≤ n ≤ 1000
- -1000 ≤ begin < finish ≤ 1000

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, dynamic-programming, greedy, sorting
