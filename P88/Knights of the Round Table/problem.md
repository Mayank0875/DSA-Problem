## Title
Knights of the Round Table

## Slug
knights-of-the-round-table

## Difficulty
Medium

## Description
Knights have different valor scores. To embark on the Holy Grail quest, a party must possess more than half the total valor of the table.

Your task is to count the number of **quest partiess**. A quest party is considered valid if it satisfies two specific criteria:
1.  **Quest Approval:** The total valor of the quest party is strictly greater than half of the total valor across all knights.
2.  **No Superfluous knights:** The quest party is minimal. This means that removing **any one** knight from the quest party would cause the remaining total to drop to half or less of the total valor (losing the Quest Approval).

## Examples

### 1

#### Input
5
3 1 4 1 5

#### Output
4

#### Explanation
Total valor is 14. Half is 7. We need a sum > 7.
The group {5, 4, 1} (Sum 10) is **not** valid because removing 1 leaves 9, which is still > 7.
Valid groups are those where every member is critical.

### 2

#### Input
4
1 2 3 4

#### Output
3

#### Explanation
Total valor = 10. Half = 5.
Valid quest partiess: {4, 2}, {4, 3}, {3, 2, 1}.

## Input Format
- The first line contains an integer n: the number of knights.
- The second line contains n integers: the valor of each knight.

## Output Format
- Return one integer: the total number of valid quest partiess.

## Constraints
- 1 ≤ n ≤ 60
- 1 ≤ valor ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths, dynamic-programming
