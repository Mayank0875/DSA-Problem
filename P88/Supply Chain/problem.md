## Title
Supply Chain

## Slug
supply-chain

## Difficulty
Medium

## Description
Suppliers provide different quantities of raw material. A production halt occurs if a striking group of suppliers controls more than half the total supply.

Your task is to count the number of **strikess**. A strike is considered valid if it satisfies two specific criteria:
1.  **Supply Shock:** The total quantity of the strike is strictly greater than half of the total quantity across all suppliers.
2.  **No Superfluous suppliers:** The strike is minimal. This means that removing **any one** supplier from the strike would cause the remaining total to drop to half or less of the total quantity (losing the Supply Shock).

## Examples

### 1

#### Input
5
3 1 4 1 5

#### Output
4

#### Explanation
Total quantity is 14. Half is 7. We need a sum > 7.
The group {5, 4, 1} (Sum 10) is **not** valid because removing 1 leaves 9, which is still > 7.
Valid groups are those where every member is critical.

### 2

#### Input
4
1 2 3 4

#### Output
3

#### Explanation
Total quantity = 10. Half = 5.
Valid strikess: {4, 2}, {4, 3}, {3, 2, 1}.

## Input Format
- The first line contains an integer n: the number of suppliers.
- The second line contains n integers: the quantity of each supplier.

## Output Format
- Return one integer: the total number of valid strikess.

## Constraints
- 1 ≤ n ≤ 60
- 1 ≤ quantity ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths, dynamic-programming
