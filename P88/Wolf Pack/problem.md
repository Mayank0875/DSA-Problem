## Title
Wolf Pack

## Slug
wolf-pack

## Difficulty
Medium

## Description
Wolves in a pack have different strength levels. To take down a massive prey, a hunting party needs more than half the total strength of the pack.

Your task is to count the number of **hunting partiess**. A hunting party is considered valid if it satisfies two specific criteria:
1.  **Takedown Power:** The total strength of the hunting party is strictly greater than half of the total strength across all wolves.
2.  **No Superfluous wolves:** The hunting party is minimal. This means that removing **any one** wolf from the hunting party would cause the remaining total to drop to half or less of the total strength (losing the Takedown Power).

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
Valid hunting partiess: {4, 2}, {4, 3}, {3, 2, 1}.

## Input Format
- The first line contains an integer n: the number of wolves.
- The second line contains n integers: the strength of each wolf.

## Output Format
- Return one integer: the total number of valid hunting partiess.

## Constraints
- 1 ≤ n ≤ 60
- 1 ≤ strength ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths, dynamic-programming
