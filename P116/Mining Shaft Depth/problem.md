## Title
Mining Shaft Depth

## Slug
mining-shaft-depth

## Difficulty
Medium

## Description
Miners dig vertical shafts. Each planned excavation section has a top depth and bottom depth.

Plans show list of sections, each defined by a top depth and an bottom depth, represented as a pair `[top, bottom]`.

Sections must be structurally distinct. The bottom depth of an upper section must be strictly less than the top depth of the next deeper section. Specifically, to transition from section `[a, b]` to a subsequent section `[c, d]`, the bottom of the first section must be **strictly less than** the top of the second section (i.e., `b < c`).

You can select sections in any order you like to form a valid shaft plan. Your goal is to determine the maximum number of sections that can be included in a single shaft plan.

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
The longest shaft plan is `[1, 2] -> [3, 4]`. You cannot include `[2, 3]` because `2` (end of first) is not strictly less than `2` (start of second).

### 2

#### Input
3
1 2
7 8
4 5

#### Output
3

#### Explanation
The sections can be reordered to form the shaft plan `[1, 2] -> [4, 5] -> [7, 8]`. All transitions satisfy `end < start`.

## Input Format
- The first line contains an integer `n`, the number of available sections.
- The next `n` lines each contain two integers, representing the `top` and `bottom` of an section.

## Output Format
- Return a single integer representing the maximum length of the shaft plan.

## Constraints
- 1 ≤ n ≤ 1000
- -1000 ≤ top < bottom ≤ 1000

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, dynamic-programming, greedy, sorting
