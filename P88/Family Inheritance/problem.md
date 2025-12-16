## Title
Family Inheritance

## Slug
family-inheritance

## Difficulty
Medium

## Description
Heirs have different shares of an estate. To sell the family mansion, a coalition of heirs owning more than half the estate's value must agree.

Your task is to count the number of **agreementss**. A agreement is considered valid if it satisfies two specific criteria:
1.  **Majority Ownership:** The total share percentage of the agreement is strictly greater than half of the total share percentage across all heirs.
2.  **No Superfluous heirs:** The agreement is minimal. This means that removing **any one** heir from the agreement would cause the remaining total to drop to half or less of the total share percentage (losing the Majority Ownership).

## Examples

### 1

#### Input
5
3 1 4 1 5

#### Output
4

#### Explanation
Total share percentage is 14. Half is 7. We need a sum > 7.
The group {5, 4, 1} (Sum 10) is **not** valid because removing 1 leaves 9, which is still > 7.
Valid groups are those where every member is critical.

### 2

#### Input
4
1 2 3 4

#### Output
3

#### Explanation
Total share percentage = 10. Half = 5.
Valid agreementss: {4, 2}, {4, 3}, {3, 2, 1}.

## Input Format
- The first line contains an integer n: the number of heirs.
- The second line contains n integers: the share percentage of each heir.

## Output Format
- Return one integer: the total number of valid agreementss.

## Constraints
- 1 ≤ n ≤ 60
- 1 ≤ share percentage ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths, dynamic-programming
