## Title
Rocket Thrust

## Slug
rocket-thrust

## Difficulty
Medium

## Description
A rocket has multiple engines with different thrust values. To achieve escape velocity, a combination of active engines must provide more than half the total potential thrust.

Your task is to count the number of **configurationss**. A configuration is considered valid if it satisfies two specific criteria:
1.  **Escape Thrust:** The total thrust of the configuration is strictly greater than half of the total thrust across all engines.
2.  **No Superfluous engines:** The configuration is minimal. This means that removing **any one** engine from the configuration would cause the remaining total to drop to half or less of the total thrust (losing the Escape Thrust).

## Examples

### 1

#### Input
5
3 1 4 1 5

#### Output
4

#### Explanation
Total thrust is 14. Half is 7. We need a sum > 7.
The group {5, 4, 1} (Sum 10) is **not** valid because removing 1 leaves 9, which is still > 7.
Valid groups are those where every member is critical.

### 2

#### Input
4
1 2 3 4

#### Output
3

#### Explanation
Total thrust = 10. Half = 5.
Valid configurationss: {4, 2}, {4, 3}, {3, 2, 1}.

## Input Format
- The first line contains an integer n: the number of engines.
- The second line contains n integers: the thrust of each engine.

## Output Format
- Return one integer: the total number of valid configurationss.

## Constraints
- 1 ≤ n ≤ 60
- 1 ≤ thrust ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths, dynamic-programming
