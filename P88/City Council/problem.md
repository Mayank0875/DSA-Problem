## Title
City Council

## Slug
city-council

## Difficulty
Medium

## Description
Council members represent districts with different populations. A motion passes if the supporting members represent a majority of the total city population.

Your task is to count the number of **majoritiess**. A majority is considered valid if it satisfies two specific criteria:
1.  **Motion Pass:** The total population of the majority is strictly greater than half of the total population across all members.
2.  **No Superfluous members:** The majority is minimal. This means that removing **any one** member from the majority would cause the remaining total to drop to half or less of the total population (losing the Motion Pass).

## Examples

### 1

#### Input
5
3 1 4 1 5

#### Output
4

#### Explanation
Total population is 14. Half is 7. We need a sum > 7.
The group {5, 4, 1} (Sum 10) is **not** valid because removing 1 leaves 9, which is still > 7.
Valid groups are those where every member is critical.

### 2

#### Input
4
1 2 3 4

#### Output
3

#### Explanation
Total population = 10. Half = 5.
Valid majoritiess: {4, 2}, {4, 3}, {3, 2, 1}.

## Input Format
- The first line contains an integer n: the number of members.
- The second line contains n integers: the population of each member.

## Output Format
- Return one integer: the total number of valid majoritiess.

## Constraints
- 1 ≤ n ≤ 60
- 1 ≤ population ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths, dynamic-programming
