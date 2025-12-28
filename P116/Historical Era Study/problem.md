## Title
Historical Era Study

## Slug
historical-era-study

## Difficulty
Medium

## Description
A historian studies eras. Each era covers a range of years.

The timeline has list of eras, each defined by a start year and an end year, represented as a pair `[start, end]`.

To study cause and effect, the historian must finish one era strictly before starting the study of the next era. Specifically, to transition from era `[a, b]` to a subsequent era `[c, d]`, the end of the first era must be **strictly less than** the start of the second era (i.e., `b < c`).

You can select eras in any order you like to form a valid curriculum. Your goal is to determine the maximum number of eras that can be included in a single curriculum.

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
The longest curriculum is `[1, 2] -> [3, 4]`. You cannot include `[2, 3]` because `2` (end of first) is not strictly less than `2` (start of second).

### 2

#### Input
3
1 2
7 8
4 5

#### Output
3

#### Explanation
The eras can be reordered to form the curriculum `[1, 2] -> [4, 5] -> [7, 8]`. All transitions satisfy `end < start`.

## Input Format
- The first line contains an integer `n`, the number of available eras.
- The next `n` lines each contain two integers, representing the `start` and `end` of an era.

## Output Format
- Return a single integer representing the maximum length of the curriculum.

## Constraints
- 1 ≤ n ≤ 1000
- -1000 ≤ start < end ≤ 1000

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, dynamic-programming, greedy, sorting
