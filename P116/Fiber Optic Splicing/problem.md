## Title
Fiber Optic Splicing

## Slug
fiber-optic-splicing

## Difficulty
Medium

## Description
Technicians splice cables. Each splice job happens between two distance markers on the line.

Job tickets list list of splices, each defined by a start marker and an end marker, represented as a pair `[start, end]`.

Work crews need separation. The end marker of one splice must be strictly less than the start marker of the next. Specifically, to transition from splice `[a, b]` to a subsequent splice `[c, d]`, the end of the first splice must be **strictly less than** the start of the second splice (i.e., `b < c`).

You can select splices in any order you like to form a valid job list. Your goal is to determine the maximum number of splices that can be included in a single job list.

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
The longest job list is `[1, 2] -> [3, 4]`. You cannot include `[2, 3]` because `2` (end of first) is not strictly less than `2` (start of second).

### 2

#### Input
3
1 2
7 8
4 5

#### Output
3

#### Explanation
The splices can be reordered to form the job list `[1, 2] -> [4, 5] -> [7, 8]`. All transitions satisfy `end < start`.

## Input Format
- The first line contains an integer `n`, the number of available splices.
- The next `n` lines each contain two integers, representing the `start` and `end` of an splice.

## Output Format
- Return a single integer representing the maximum length of the job list.

## Constraints
- 1 ≤ n ≤ 1000
- -1000 ≤ start < end ≤ 1000

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, dynamic-programming, greedy, sorting
