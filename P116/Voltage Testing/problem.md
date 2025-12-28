## Title
Voltage Testing

## Slug
voltage-testing

## Difficulty
Medium

## Description
Components are tested at voltage ranges. Each test has a low V and high V.

The protocol lists list of tests, each defined by a low V and an high V, represented as a pair `[lo, hi]`.

To ramp up safely, the high voltage of one test must be strictly less than the low voltage of the next. Specifically, to transition from test `[a, b]` to a subsequent test `[c, d]`, the hi of the first test must be **strictly less than** the lo of the second test (i.e., `b < c`).

You can select tests in any order you like to form a valid test suite. Your goal is to determine the maximum number of tests that can be included in a single test suite.

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
The longest test suite is `[1, 2] -> [3, 4]`. You cannot include `[2, 3]` because `2` (end of first) is not strictly less than `2` (start of second).

### 2

#### Input
3
1 2
7 8
4 5

#### Output
3

#### Explanation
The tests can be reordered to form the test suite `[1, 2] -> [4, 5] -> [7, 8]`. All transitions satisfy `end < start`.

## Input Format
- The first line contains an integer `n`, the number of available tests.
- The next `n` lines each contain two integers, representing the `lo` and `hi` of an test.

## Output Format
- Return a single integer representing the maximum length of the test suite.

## Constraints
- 1 ≤ n ≤ 1000
- -1000 ≤ lo < hi ≤ 1000

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, dynamic-programming, greedy, sorting
