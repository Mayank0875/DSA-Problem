## Title
Scholarship Eligibility

## Slug
scholarship-eligibility

## Difficulty
Medium

## Description
A student applies for grants. Each grant covers a specific GPA range.

Available grants are list of grants, each defined by a min GPA and an max GPA, represented as a pair `[min, max]`.

To stack non-conflicting awards (logic stretch), the max GPA of one tier must be strictly less than the min GPA of the next tier. Specifically, to transition from grant `[a, b]` to a subsequent grant `[c, d]`, the max of the first grant must be **strictly less than** the min of the second grant (i.e., `b < c`).

You can select grants in any order you like to form a valid award list. Your goal is to determine the maximum number of grants that can be included in a single award list.

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
The longest award list is `[1, 2] -> [3, 4]`. You cannot include `[2, 3]` because `2` (end of first) is not strictly less than `2` (start of second).

### 2

#### Input
3
1 2
7 8
4 5

#### Output
3

#### Explanation
The grants can be reordered to form the award list `[1, 2] -> [4, 5] -> [7, 8]`. All transitions satisfy `end < start`.

## Input Format
- The first line contains an integer `n`, the number of available grants.
- The next `n` lines each contain two integers, representing the `min` and `max` of an grant.

## Output Format
- Return a single integer representing the maximum length of the award list.

## Constraints
- 1 ≤ n ≤ 1000
- -1000 ≤ min < max ≤ 1000

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, dynamic-programming, greedy, sorting
