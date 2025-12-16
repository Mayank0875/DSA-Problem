## Title
Gold Rush

## Slug
gold-rush

## Difficulty
Medium

## Description
Claims have different estimated gold reserves. A mining conglomerate dominates if it buys claims holding more than half the total reserves.

Your task is to count the number of **conglomeratess**. A conglomerate is considered valid if it satisfies two specific criteria:
1.  **Market Dominance:** The total gold reserve of the conglomerate is strictly greater than half of the total gold reserve across all claims.
2.  **No Superfluous claims:** The conglomerate is minimal. This means that removing **any one** claim from the conglomerate would cause the remaining total to drop to half or less of the total gold reserve (losing the Market Dominance).

## Examples

### 1

#### Input
5
3 1 4 1 5

#### Output
4

#### Explanation
Total gold reserve is 14. Half is 7. We need a sum > 7.
The group {5, 4, 1} (Sum 10) is **not** valid because removing 1 leaves 9, which is still > 7.
Valid groups are those where every member is critical.

### 2

#### Input
4
1 2 3 4

#### Output
3

#### Explanation
Total gold reserve = 10. Half = 5.
Valid conglomeratess: {4, 2}, {4, 3}, {3, 2, 1}.

## Input Format
- The first line contains an integer n: the number of claims.
- The second line contains n integers: the gold reserve of each claim.

## Output Format
- Return one integer: the total number of valid conglomeratess.

## Constraints
- 1 ≤ n ≤ 60
- 1 ≤ gold reserve ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths, dynamic-programming
