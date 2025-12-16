## Title
Sports League

## Slug
sports-league

## Difficulty
Medium

## Description
Teams have fanbases of different sizes. A new rule passes if teams representing a majority of the total fanbase agree.

Your task is to count the number of **blocss**. A bloc is considered valid if it satisfies two specific criteria:
1.  **Rule Change:** The total fanbase size of the bloc is strictly greater than half of the total fanbase size across all teams.
2.  **No Superfluous teams:** The bloc is minimal. This means that removing **any one** team from the bloc would cause the remaining total to drop to half or less of the total fanbase size (losing the Rule Change).

## Examples

### 1

#### Input
5
3 1 4 1 5

#### Output
4

#### Explanation
Total fanbase size is 14. Half is 7. We need a sum > 7.
The group {5, 4, 1} (Sum 10) is **not** valid because removing 1 leaves 9, which is still > 7.
Valid groups are those where every member is critical.

### 2

#### Input
4
1 2 3 4

#### Output
3

#### Explanation
Total fanbase size = 10. Half = 5.
Valid blocss: {4, 2}, {4, 3}, {3, 2, 1}.

## Input Format
- The first line contains an integer n: the number of teams.
- The second line contains n integers: the fanbase size of each team.

## Output Format
- Return one integer: the total number of valid blocss.

## Constraints
- 1 ≤ n ≤ 60
- 1 ≤ fanbase size ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths, dynamic-programming
