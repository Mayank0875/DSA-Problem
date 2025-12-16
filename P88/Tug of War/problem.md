## Title
Tug of War

## Slug
tug-of-war

## Difficulty
Medium

## Description
A group of athletes with different strength ratings wants to form a team. To win against the rest of the world, the team's total strength must exceed half the total strength of all athletes combined.

Your task is to count the number of **teamss**. A team is considered valid if it satisfies two specific criteria:
1.  **Dominance:** The total strength of the team is strictly greater than half of the total strength across all athletes.
2.  **No Superfluous athletes:** The team is minimal. This means that removing **any one** athlete from the team would cause the remaining total to drop to half or less of the total strength (losing the Dominance).

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
Valid teamss: {4, 2}, {4, 3}, {3, 2, 1}.

## Input Format
- The first line contains an integer n: the number of athletes.
- The second line contains n integers: the strength of each athlete.

## Output Format
- Return one integer: the total number of valid teamss.

## Constraints
- 1 ≤ n ≤ 60
- 1 ≤ strength ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths, dynamic-programming
