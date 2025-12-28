## Title
Software Versioning

## Slug
software-versioning

## Difficulty
Medium

## Description
Updates are released. Each version is valid from a start build number to an end build number.

The repo has list of versions, each defined by a start build and an end build, represented as a pair `[start, end]`.

To ensure a clean upgrade path, the end build of the current version must be strictly less than the start build of the next. Specifically, to transition from version `[a, b]` to a subsequent version `[c, d]`, the end of the first version must be **strictly less than** the start of the second version (i.e., `b < c`).

You can select versions in any order you like to form a valid release chain. Your goal is to determine the maximum number of versions that can be included in a single release chain.

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
The longest release chain is `[1, 2] -> [3, 4]`. You cannot include `[2, 3]` because `2` (end of first) is not strictly less than `2` (start of second).

### 2

#### Input
3
1 2
7 8
4 5

#### Output
3

#### Explanation
The versions can be reordered to form the release chain `[1, 2] -> [4, 5] -> [7, 8]`. All transitions satisfy `end < start`.

## Input Format
- The first line contains an integer `n`, the number of available versions.
- The next `n` lines each contain two integers, representing the `start` and `end` of an version.

## Output Format
- Return a single integer representing the maximum length of the release chain.

## Constraints
- 1 ≤ n ≤ 1000
- -1000 ≤ start < end ≤ 1000

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, dynamic-programming, greedy, sorting
