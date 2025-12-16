## Title
Machine Learning Ensemble

## Slug
machine-learning-ensemble

## Difficulty
Medium

## Description
An ensemble of models has different accuracy weights. To make a final prediction, a subset of models must have a combined weight greater than half the total.

Your task is to count the number of **ensembless**. A ensemble is considered valid if it satisfies two specific criteria:
1.  **Prediction Confidence:** The total accuracy weight of the ensemble is strictly greater than half of the total accuracy weight across all models.
2.  **No Superfluous models:** The ensemble is minimal. This means that removing **any one** model from the ensemble would cause the remaining total to drop to half or less of the total accuracy weight (losing the Prediction Confidence).

## Examples

### 1

#### Input
5
3 1 4 1 5

#### Output
4

#### Explanation
Total accuracy weight is 14. Half is 7. We need a sum > 7.
The group {5, 4, 1} (Sum 10) is **not** valid because removing 1 leaves 9, which is still > 7.
Valid groups are those where every member is critical.

### 2

#### Input
4
1 2 3 4

#### Output
3

#### Explanation
Total accuracy weight = 10. Half = 5.
Valid ensembless: {4, 2}, {4, 3}, {3, 2, 1}.

## Input Format
- The first line contains an integer n: the number of models.
- The second line contains n integers: the accuracy weight of each model.

## Output Format
- Return one integer: the total number of valid ensembless.

## Constraints
- 1 ≤ n ≤ 60
- 1 ≤ accuracy weight ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths, dynamic-programming
