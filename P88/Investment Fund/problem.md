## Title
Investment Fund

## Slug
investment-fund

## Difficulty
Medium

## Description
Investors pool their capital. To take control of the fund's direction, a group must own more than 50% of the total capital.

Your task is to count the number of **control groupss**. A control group is considered valid if it satisfies two specific criteria:
1.  **Controlling Interest:** The total capital of the control group is strictly greater than half of the total capital across all investors.
2.  **No Superfluous investors:** The control group is minimal. This means that removing **any one** investor from the control group would cause the remaining total to drop to half or less of the total capital (losing the Controlling Interest).

## Examples

### 1

#### Input
5
3 1 4 1 5

#### Output
4

#### Explanation
Total capital is 14. Half is 7. We need a sum > 7.
The group {5, 4, 1} (Sum 10) is **not** valid because removing 1 leaves 9, which is still > 7.
Valid groups are those where every member is critical.

### 2

#### Input
4
1 2 3 4

#### Output
3

#### Explanation
Total capital = 10. Half = 5.
Valid control groupss: {4, 2}, {4, 3}, {3, 2, 1}.

## Input Format
- The first line contains an integer n: the number of investors.
- The second line contains n integers: the capital of each investor.

## Output Format
- Return one integer: the total number of valid control groupss.

## Constraints
- 1 ≤ n ≤ 60
- 1 ≤ capital ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths, dynamic-programming
