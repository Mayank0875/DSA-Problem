## Title
Medieval Council

## Slug
medieval-council

## Difficulty
Medium

## Description
The King's council consists of lords with varying influence points. To approve a decree, a coalition of lords must wield more than half the total influence of the realm.

Your task is to count the number of **coalitionss**. A coalition is considered valid if it satisfies two specific criteria:
1.  **Royal Decree:** The total influence of the coalition is strictly greater than half of the total influence across all lords.
2.  **No Superfluous lords:** The coalition is minimal. This means that removing **any one** lord from the coalition would cause the remaining total to drop to half or less of the total influence (losing the Royal Decree).

## Examples

### 1

#### Input
5
3 1 4 1 5

#### Output
4

#### Explanation
Total influence is 14. Half is 7. We need a sum > 7.
The group {5, 4, 1} (Sum 10) is **not** valid because removing 1 leaves 9, which is still > 7.
Valid groups are those where every member is critical.

### 2

#### Input
4
1 2 3 4

#### Output
3

#### Explanation
Total influence = 10. Half = 5.
Valid coalitionss: {4, 2}, {4, 3}, {3, 2, 1}.

## Input Format
- The first line contains an integer n: the number of lords.
- The second line contains n integers: the influence of each lord.

## Output Format
- Return one integer: the total number of valid coalitionss.

## Constraints
- 1 ≤ n ≤ 60
- 1 ≤ influence ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths, dynamic-programming
