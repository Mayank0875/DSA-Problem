## Title
Deep Sea Diving

## Slug
deep-sea-diving

## Difficulty
Medium

## Description
A diver explores depth ranges. Each dive covers a min depth and max depth.

Dive plan: list of dives, each defined by a min depth and an max depth, represented as a pair `[min, max]`.

To decompress safely between deeper dives, the max depth of a shallower dive must be strictly less (numerically) than the min depth of the next deep dive. Specifically, to transition from dive `[a, b]` to a subsequent dive `[c, d]`, the max of the first dive must be **strictly less than** the min of the second dive (i.e., `b < c`).

You can select dives in any order you like to form a valid dive log. Your goal is to determine the maximum number of dives that can be included in a single dive log.

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
The longest dive log is `[1, 2] -> [3, 4]`. You cannot include `[2, 3]` because `2` (end of first) is not strictly less than `2` (start of second).

### 2

#### Input
3
1 2
7 8
4 5

#### Output
3

#### Explanation
The dives can be reordered to form the dive log `[1, 2] -> [4, 5] -> [7, 8]`. All transitions satisfy `end < start`.

## Input Format
- The first line contains an integer `n`, the number of available dives.
- The next `n` lines each contain two integers, representing the `min` and `max` of an dive.

## Output Format
- Return a single integer representing the maximum length of the dive log.

## Constraints
- 1 ≤ n ≤ 1000
- -1000 ≤ min < max ≤ 1000

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, dynamic-programming, greedy, sorting
