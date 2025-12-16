## Title
Military Alliance

## Slug
military-alliance

## Difficulty
Medium

## Description
Nations with different military strengths want to form an alliance. An alliance is considered 'Global Superpower' only if its combined strength exceeds half the world's total military strength.

Your task is to count the number of **alliancess**. A alliance is considered valid if it satisfies two specific criteria:
1.  **Superpower Status:** The total strength of the alliance is strictly greater than half of the total strength across all nations.
2.  **No Superfluous nations:** The alliance is minimal. This means that removing **any one** nation from the alliance would cause the remaining total to drop to half or less of the total strength (losing the Superpower Status).

## Examples

### 1

#### Input
5
3 1 4 1 5

#### Output
4

#### Explanation
Total strength is 14. Half is 7. We need a sum > 7.
The group {5, 4, 1} (Sum 10) is **not** valid because removing 1 leaves 9, which is still > 7.
Valid groups are those where every member is critical.

### 2

#### Input
4
1 2 3 4

#### Output
3

#### Explanation
Total strength = 10. Half = 5.
Valid alliancess: {4, 2}, {4, 3}, {3, 2, 1}.

## Input Format
- The first line contains an integer n: the number of nations.
- The second line contains n integers: the strength of each nation.

## Output Format
- Return one integer: the total number of valid alliancess.

## Constraints
- 1 ≤ n ≤ 60
- 1 ≤ strength ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths, dynamic-programming
