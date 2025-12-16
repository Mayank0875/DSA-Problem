## Title
Software Feature Vote

## Slug
software-feature-vote

## Difficulty
Medium

## Description
Users vote on features with 'karma points'. A feature is prioritized only if the users supporting it hold a majority of the total karma points in the system.

Your task is to count the number of **supporter groupss**. A supporter group is considered valid if it satisfies two specific criteria:
1.  **Priority Status:** The total karma of the supporter group is strictly greater than half of the total karma across all users.
2.  **No Superfluous users:** The supporter group is minimal. This means that removing **any one** user from the supporter group would cause the remaining total to drop to half or less of the total karma (losing the Priority Status).

## Examples

### 1

#### Input
5
3 1 4 1 5

#### Output
4

#### Explanation
Total karma is 14. Half is 7. We need a sum > 7.
The group {5, 4, 1} (Sum 10) is **not** valid because removing 1 leaves 9, which is still > 7.
Valid groups are those where every member is critical.

### 2

#### Input
4
1 2 3 4

#### Output
3

#### Explanation
Total karma = 10. Half = 5.
Valid supporter groupss: {4, 2}, {4, 3}, {3, 2, 1}.

## Input Format
- The first line contains an integer n: the number of users.
- The second line contains n integers: the karma of each user.

## Output Format
- Return one integer: the total number of valid supporter groupss.

## Constraints
- 1 ≤ n ≤ 60
- 1 ≤ karma ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths, dynamic-programming
