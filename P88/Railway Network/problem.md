## Title
Railway Network

## Slug
railway-network

## Difficulty
Medium

## Description
Lines have different passenger capacities. The system gridlocks if a set of overloaded lines accounts for more than half the total capacity.

Your task is to count the number of **failuress**. A failure is considered valid if it satisfies two specific criteria:
1.  **Gridlock:** The total capacity of the failure is strictly greater than half of the total capacity across all lines.
2.  **No Superfluous lines:** The failure is minimal. This means that removing **any one** line from the failure would cause the remaining total to drop to half or less of the total capacity (losing the Gridlock).

## Examples

### 1

#### Input
5
3 1 4 1 5

#### Output
4

#### Explanation
Total capacity is 14. Half is 7. We need a sum > 7.
The group {5, 4, 1} (Sum 10) is **not** valid because removing 1 leaves 9, which is still > 7.
Valid groups are those where every member is critical.

### 2

#### Input
4
1 2 3 4

#### Output
3

#### Explanation
Total capacity = 10. Half = 5.
Valid failuress: {4, 2}, {4, 3}, {3, 2, 1}.

## Input Format
- The first line contains an integer n: the number of lines.
- The second line contains n integers: the capacity of each line.

## Output Format
- Return one integer: the total number of valid failuress.

## Constraints
- 1 ≤ n ≤ 60
- 1 ≤ capacity ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths, dynamic-programming
