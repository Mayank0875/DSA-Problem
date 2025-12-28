## Title
Fireworks Display

## Slug
fireworks-display

## Difficulty
Medium

## Description
Pyrotechnics are timed. Each shell has a launch time and explosion time.

The script lists list of shells, each defined by a launch and an bang, represented as a pair `[L, B]`.

For visual clarity, a shell must explode strictly before the next launch occurs. Specifically, to transition from shell `[a, b]` to a subsequent shell `[c, d]`, the B of the first shell must be **strictly less than** the L of the second shell (i.e., `b < c`).

You can select shells in any order you like to form a valid show. Your goal is to determine the maximum number of shells that can be included in a single show.

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
The longest show is `[1, 2] -> [3, 4]`. You cannot include `[2, 3]` because `2` (end of first) is not strictly less than `2` (start of second).

### 2

#### Input
3
1 2
7 8
4 5

#### Output
3

#### Explanation
The shells can be reordered to form the show `[1, 2] -> [4, 5] -> [7, 8]`. All transitions satisfy `end < start`.

## Input Format
- The first line contains an integer `n`, the number of available shells.
- The next `n` lines each contain two integers, representing the `L` and `B` of an shell.

## Output Format
- Return a single integer representing the maximum length of the show.

## Constraints
- 1 ≤ n ≤ 1000
- -1000 ≤ L < B ≤ 1000

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, dynamic-programming, greedy, sorting
