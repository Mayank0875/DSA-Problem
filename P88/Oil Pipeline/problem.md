## Title
Oil Pipeline

## Slug
oil-pipeline

## Difficulty
Medium

## Description
Pipes have different flow capacities. To rupture the main valve, the active pipes must carry more than half the total system pressure.

Your task is to count the number of **configurationss**. A configuration is considered valid if it satisfies two specific criteria:
1.  **Rupture Point:** The total pressure of the configuration is strictly greater than half of the total pressure across all pipes.
2.  **No Superfluous pipes:** The configuration is minimal. This means that removing **any one** pipe from the configuration would cause the remaining total to drop to half or less of the total pressure (losing the Rupture Point).

## Examples

### 1

#### Input
5
3 1 4 1 5

#### Output
4

#### Explanation
Total pressure is 14. Half is 7. We need a sum > 7.
The group {5, 4, 1} (Sum 10) is **not** valid because removing 1 leaves 9, which is still > 7.
Valid groups are those where every member is critical.

### 2

#### Input
4
1 2 3 4

#### Output
3

#### Explanation
Total pressure = 10. Half = 5.
Valid configurationss: {4, 2}, {4, 3}, {3, 2, 1}.

## Input Format
- The first line contains an integer n: the number of pipes.
- The second line contains n integers: the pressure of each pipe.

## Output Format
- Return one integer: the total number of valid configurationss.

## Constraints
- 1 ≤ n ≤ 60
- 1 ≤ pressure ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths, dynamic-programming
