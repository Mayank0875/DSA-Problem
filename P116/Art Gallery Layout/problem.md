## Title
Art Gallery Layout

## Slug
art-gallery-layout

## Difficulty
Medium

## Description
Paintings are hung on a wall. Each frame occupies a horizontal range from left to right.

The collection has list of paintings, each defined by a left edge and an right edge, represented as a pair `[left, right]`.

Paintings cannot overlap. The right edge of one frame must be strictly less than the left edge of the next. Specifically, to transition from painting `[a, b]` to a subsequent painting `[c, d]`, the right of the first painting must be **strictly less than** the left of the second painting (i.e., `b < c`).

You can select paintings in any order you like to form a valid exhibit. Your goal is to determine the maximum number of paintings that can be included in a single exhibit.

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
The longest exhibit is `[1, 2] -> [3, 4]`. You cannot include `[2, 3]` because `2` (end of first) is not strictly less than `2` (start of second).

### 2

#### Input
3
1 2
7 8
4 5

#### Output
3

#### Explanation
The paintings can be reordered to form the exhibit `[1, 2] -> [4, 5] -> [7, 8]`. All transitions satisfy `end < start`.

## Input Format
- The first line contains an integer `n`, the number of available paintings.
- The next `n` lines each contain two integers, representing the `left` and `right` of an painting.

## Output Format
- Return a single integer representing the maximum length of the exhibit.

## Constraints
- 1 ≤ n ≤ 1000
- -1000 ≤ left < right ≤ 1000

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, dynamic-programming, greedy, sorting
