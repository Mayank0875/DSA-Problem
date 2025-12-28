## Title
Train Yard Switching

## Slug
train-yard-switching

## Difficulty
Medium

## Description
A switcher engine moves cars. Each move occupies a track section start/end.

Operations list list of moves, each defined by a start track and an end track, represented as a pair `[start, end]`.

To prevent collisions, the end track of one move must be strictly less than the start track of the next. Specifically, to transition from move `[a, b]` to a subsequent move `[c, d]`, the end of the first move must be **strictly less than** the start of the second move (i.e., `b < c`).

You can select moves in any order you like to form a valid switch list. Your goal is to determine the maximum number of moves that can be included in a single switch list.

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
The longest switch list is `[1, 2] -> [3, 4]`. You cannot include `[2, 3]` because `2` (end of first) is not strictly less than `2` (start of second).

### 2

#### Input
3
1 2
7 8
4 5

#### Output
3

#### Explanation
The moves can be reordered to form the switch list `[1, 2] -> [4, 5] -> [7, 8]`. All transitions satisfy `end < start`.

## Input Format
- The first line contains an integer `n`, the number of available moves.
- The next `n` lines each contain two integers, representing the `start` and `end` of an move.

## Output Format
- Return a single integer representing the maximum length of the switch list.

## Constraints
- 1 ≤ n ≤ 1000
- -1000 ≤ start < end ≤ 1000

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, dynamic-programming, greedy, sorting
