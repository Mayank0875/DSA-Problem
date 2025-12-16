## Title
Galactic Senate

## Slug
galactic-senate

## Difficulty
Medium

## Description
Planets have voting power based on their population. To pass a galactic law, a coalition of planets must hold a strict majority of the total votes.

Your task is to count the number of **coalitionss**. A coalition is considered valid if it satisfies two specific criteria:
1.  **Galactic Law:** The total votes of the coalition is strictly greater than half of the total votes across all planets.
2.  **No Superfluous planets:** The coalition is minimal. This means that removing **any one** planet from the coalition would cause the remaining total to drop to half or less of the total votes (losing the Galactic Law).

## Examples

### 1

#### Input
5
3 1 4 1 5

#### Output
4

#### Explanation
Total votes is 14. Half is 7. We need a sum > 7.
The group {5, 4, 1} (Sum 10) is **not** valid because removing 1 leaves 9, which is still > 7.
Valid groups are those where every member is critical.

### 2

#### Input
4
1 2 3 4

#### Output
3

#### Explanation
Total votes = 10. Half = 5.
Valid coalitionss: {4, 2}, {4, 3}, {3, 2, 1}.

## Input Format
- The first line contains an integer n: the number of planets.
- The second line contains n integers: the votes of each planet.

## Output Format
- Return one integer: the total number of valid coalitionss.

## Constraints
- 1 ≤ n ≤ 60
- 1 ≤ votes ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths, dynamic-programming
