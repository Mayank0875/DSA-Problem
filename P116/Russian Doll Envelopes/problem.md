## Title
Russian Doll Envelopes

## Slug
russian-doll-envelopes

## Difficulty
Medium

## Description
You have a collection of envelopes of different sizes. Each envelope has a width and a height.

You have a list of envelopes, each defined by a width and an height, represented as a pair `[w, h]`.

One envelope fits inside another only if both its width and height are strictly smaller. (Simplified logic: assume we sort by width and chain by height). Wait, actually let's stick to the pair chain logic strictly: To nest envelope A inside B, the height of A must be strictly less than the width of B (simulating a specific packing rule). Specifically, to transition from envelope `[a, b]` to a subsequent envelope `[c, d]`, the h of the first envelope must be **strictly less than** the w of the second envelope (i.e., `b < c`).

You can select envelopes in any order you like to form a valid nested set. Your goal is to determine the maximum number of envelopes that can be included in a single nested set.

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
The longest nested set is `[1, 2] -> [3, 4]`. You cannot include `[2, 3]` because `2` (end of first) is not strictly less than `2` (start of second).

### 2

#### Input
3
1 2
7 8
4 5

#### Output
3

#### Explanation
The envelopes can be reordered to form the nested set `[1, 2] -> [4, 5] -> [7, 8]`. All transitions satisfy `end < start`.

## Input Format
- The first line contains an integer `n`, the number of available envelopes.
- The next `n` lines each contain two integers, representing the `w` and `h` of an envelope.

## Output Format
- Return a single integer representing the maximum length of the nested set.

## Constraints
- 1 ≤ n ≤ 1000
- -1000 ≤ w < h ≤ 1000

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, dynamic-programming, greedy, sorting
