## Title
Space Station Shields

## Slug
space-station-shields

## Difficulty
Medium

## Description
Shield generators have different output levels. To block a solar flare, active generators must output more than half the station's total shield capacity.

Your task is to count the number of **configurationss**. A configuration is considered valid if it satisfies two specific criteria:
1.  **Solar Defense:** The total output of the configuration is strictly greater than half of the total output across all generators.
2.  **No Superfluous generators:** The configuration is minimal. This means that removing **any one** generator from the configuration would cause the remaining total to drop to half or less of the total output (losing the Solar Defense).

## Examples

### 1

#### Input
5
3 1 4 1 5

#### Output
4

#### Explanation
Total output is 14. Half is 7. We need a sum > 7.
The group {5, 4, 1} (Sum 10) is **not** valid because removing 1 leaves 9, which is still > 7.
Valid groups are those where every member is critical.

### 2

#### Input
4
1 2 3 4

#### Output
3

#### Explanation
Total output = 10. Half = 5.
Valid configurationss: {4, 2}, {4, 3}, {3, 2, 1}.

## Input Format
- The first line contains an integer n: the number of generators.
- The second line contains n integers: the output of each generator.

## Output Format
- Return one integer: the total number of valid configurationss.

## Constraints
- 1 ≤ n ≤ 60
- 1 ≤ output ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths, dynamic-programming
