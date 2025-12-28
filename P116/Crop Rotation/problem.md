## Title
Crop Rotation

## Slug
crop-rotation

## Difficulty
Medium

## Description
A farmer schedules crops. Each crop requires a planting month and harvest month.

Seed packets show list of crops, each defined by a plant month and an harvest month, represented as a pair `[plant, harvest]`.

The field must be cleared. The harvest month of the previous crop must be strictly before the plant month of the next. Specifically, to transition from crop `[a, b]` to a subsequent crop `[c, d]`, the harvest of the first crop must be **strictly less than** the plant of the second crop (i.e., `b < c`).

You can select crops in any order you like to form a valid plan. Your goal is to determine the maximum number of crops that can be included in a single plan.

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
The longest plan is `[1, 2] -> [3, 4]`. You cannot include `[2, 3]` because `2` (end of first) is not strictly less than `2` (start of second).

### 2

#### Input
3
1 2
7 8
4 5

#### Output
3

#### Explanation
The crops can be reordered to form the plan `[1, 2] -> [4, 5] -> [7, 8]`. All transitions satisfy `end < start`.

## Input Format
- The first line contains an integer `n`, the number of available crops.
- The next `n` lines each contain two integers, representing the `plant` and `harvest` of an crop.

## Output Format
- Return a single integer representing the maximum length of the plan.

## Constraints
- 1 ≤ n ≤ 1000
- -1000 ≤ plant < harvest ≤ 1000

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, dynamic-programming, greedy, sorting
