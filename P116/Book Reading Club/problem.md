## Title
Book Reading Club

## Slug
book-reading-club

## Difficulty
Medium

## Description
A club reads books. Each book has a start chapter and end chapter assigned.

The list has list of assignments, each defined by a start ch and an end ch, represented as a pair `[start, end]`.

Assignments cannot overlap. The end chapter of one reading must be strictly less than the start chapter of the next. Specifically, to transition from assignment `[a, b]` to a subsequent assignment `[c, d]`, the end of the first assignment must be **strictly less than** the start of the second assignment (i.e., `b < c`).

You can select assignments in any order you like to form a valid reading plan. Your goal is to determine the maximum number of assignments that can be included in a single reading plan.

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
The longest reading plan is `[1, 2] -> [3, 4]`. You cannot include `[2, 3]` because `2` (end of first) is not strictly less than `2` (start of second).

### 2

#### Input
3
1 2
7 8
4 5

#### Output
3

#### Explanation
The assignments can be reordered to form the reading plan `[1, 2] -> [4, 5] -> [7, 8]`. All transitions satisfy `end < start`.

## Input Format
- The first line contains an integer `n`, the number of available assignments.
- The next `n` lines each contain two integers, representing the `start` and `end` of an assignment.

## Output Format
- Return a single integer representing the maximum length of the reading plan.

## Constraints
- 1 ≤ n ≤ 1000
- -1000 ≤ start < end ≤ 1000

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, dynamic-programming, greedy, sorting
