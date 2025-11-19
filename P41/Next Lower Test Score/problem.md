## Title
Next Lower Test Score

## Slug
next-lower-test-score

## Difficulty
Easy

## Description
You are a statistician analyzing student performance trends over a series of tests. For each test score, you want to find the score of the nearest future test where the class average was strictly lower. This helps identify determining factors for performance drops. Given the sequence of test scores, determine the next lower score for each data point. If performance never drops below the current level in the future, indicate this.

## Examples

### 1

#### Input
8
[73, 74, 75, 71, 69, 72, 76, 73]

#### Output
[71, 71, 71, 69, -1, -1, 73, -1]

#### Explanation
Index 0 (73): Next lower value is 71. Output 71.
Index 1 (74): Next lower value is 71. Output 71.
Index 2 (75): Next lower value is 71. Output 71.
Index 3 (71): Next lower value is 69. Output 69.
Index 4 (69): No future value is strictly lower. Output -1.
Index 5 (72): No future value is strictly lower. Output -1.
Index 6 (76): Next lower value is 73. Output 73.
Index 7 (73): No future value exists. Output -1.

### 2

#### Input
4
[30, 40, 50, 60]

#### Output
[-1, -1, -1, -1]

#### Explanation
Values are strictly increasing, so no future element has a lower value.

## Input Format
The first line contains a single integer n, the number of items.
The second line contains n space-separated integers values_0, values_1, ..., values_[n-1], representing the data sequence.

## Output Format
Return an array of integers. The i-th integer should be the value on the nearest index j > i such that values_j < values_i. If no such index exists, then -1.

## Constraints
1 ≤ n ≤ 10^5
1 ≤ values_i ≤ 10^9 for all 0 ≤ i < n.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
stack, array
