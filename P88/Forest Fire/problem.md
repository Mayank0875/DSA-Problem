## Title
Forest Fire

## Slug
forest-fire

## Difficulty
Medium

## Description
Groves of trees have different fuel loads. A fire becomes uncontrollable if the burning groves contain more than half the forest's total fuel load.

Your task is to count the number of **fire frontss**. A fire front is considered valid if it satisfies two specific criteria:
1.  **Inferno:** The total fuel load of the fire front is strictly greater than half of the total fuel load across all groves.
2.  **No Superfluous groves:** The fire front is minimal. This means that removing **any one** grove from the fire front would cause the remaining total to drop to half or less of the total fuel load (losing the Inferno).

## Examples

### 1

#### Input
5
3 1 4 1 5

#### Output
4

#### Explanation
Total fuel load is 14. Half is 7. We need a sum > 7.
The group {5, 4, 1} (Sum 10) is **not** valid because removing 1 leaves 9, which is still > 7.
Valid groups are those where every member is critical.

### 2

#### Input
4
1 2 3 4

#### Output
3

#### Explanation
Total fuel load = 10. Half = 5.
Valid fire frontss: {4, 2}, {4, 3}, {3, 2, 1}.

## Input Format
- The first line contains an integer n: the number of groves.
- The second line contains n integers: the fuel load of each grove.

## Output Format
- Return one integer: the total number of valid fire frontss.

## Constraints
- 1 ≤ n ≤ 60
- 1 ≤ fuel load ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths, dynamic-programming
