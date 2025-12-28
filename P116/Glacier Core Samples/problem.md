## Title
Glacier Core Samples

## Slug
glacier-core-samples

## Difficulty
Medium

## Description
Researchers analyze ice cores. Each sample comes from a depth range.

The freezer holds list of samples, each defined by a top depth and an bottom depth, represented as a pair `[top, bot]`.

To reconstruct the timeline, the bottom depth of a sample must be strictly less (shallower in numeric value, assuming inverted scale) than the top of the next sample. Specifically, to transition from sample `[a, b]` to a subsequent sample `[c, d]`, the bot of the first sample must be **strictly less than** the top of the second sample (i.e., `b < c`).

You can select samples in any order you like to form a valid core analysis. Your goal is to determine the maximum number of samples that can be included in a single core analysis.

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
The longest core analysis is `[1, 2] -> [3, 4]`. You cannot include `[2, 3]` because `2` (end of first) is not strictly less than `2` (start of second).

### 2

#### Input
3
1 2
7 8
4 5

#### Output
3

#### Explanation
The samples can be reordered to form the core analysis `[1, 2] -> [4, 5] -> [7, 8]`. All transitions satisfy `end < start`.

## Input Format
- The first line contains an integer `n`, the number of available samples.
- The next `n` lines each contain two integers, representing the `top` and `bot` of an sample.

## Output Format
- Return a single integer representing the maximum length of the core analysis.

## Constraints
- 1 ≤ n ≤ 1000
- -1000 ≤ top < bot ≤ 1000

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, dynamic-programming, greedy, sorting
