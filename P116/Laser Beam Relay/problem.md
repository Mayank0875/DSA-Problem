## Title
Laser Beam Relay

## Slug
laser-beam-relay

## Difficulty
Medium

## Description
Mirrors reflect a laser. Each mirror handles a specific frequency range input and output.

The setup has list of mirrors, each defined by a input freq and an output freq, represented as a pair `[in, out]`.

To step up the energy, the output frequency of one mirror must be strictly less than the input frequency of the next. Specifically, to transition from mirror `[a, b]` to a subsequent mirror `[c, d]`, the out of the first mirror must be **strictly less than** the in of the second mirror (i.e., `b < c`).

You can select mirrors in any order you like to form a valid beam path. Your goal is to determine the maximum number of mirrors that can be included in a single beam path.

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
The longest beam path is `[1, 2] -> [3, 4]`. You cannot include `[2, 3]` because `2` (end of first) is not strictly less than `2` (start of second).

### 2

#### Input
3
1 2
7 8
4 5

#### Output
3

#### Explanation
The mirrors can be reordered to form the beam path `[1, 2] -> [4, 5] -> [7, 8]`. All transitions satisfy `end < start`.

## Input Format
- The first line contains an integer `n`, the number of available mirrors.
- The next `n` lines each contain two integers, representing the `in` and `out` of an mirror.

## Output Format
- Return a single integer representing the maximum length of the beam path.

## Constraints
- 1 ≤ n ≤ 1000
- -1000 ≤ in < out ≤ 1000

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, dynamic-programming, greedy, sorting
