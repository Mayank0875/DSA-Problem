## Title
Water Reservoir

## Slug
water-reservoir

## Difficulty
Medium

## Description
Dams feed into a reservoir with different flow rates. To overflow the reservoir, a combination of open dams must provide more than half the total possible flow.

Your task is to count the number of **combinationss**. A combination is considered valid if it satisfies two specific criteria:
1.  **Overflow State:** The total flow rate of the combination is strictly greater than half of the total flow rate across all dams.
2.  **No Superfluous dams:** The combination is minimal. This means that removing **any one** dam from the combination would cause the remaining total to drop to half or less of the total flow rate (losing the Overflow State).

## Examples

### 1

#### Input
5
3 1 4 1 5

#### Output
4

#### Explanation
Total flow rate is 14. Half is 7. We need a sum > 7.
The group {5, 4, 1} (Sum 10) is **not** valid because removing 1 leaves 9, which is still > 7.
Valid groups are those where every member is critical.

### 2

#### Input
4
1 2 3 4

#### Output
3

#### Explanation
Total flow rate = 10. Half = 5.
Valid combinationss: {4, 2}, {4, 3}, {3, 2, 1}.

## Input Format
- The first line contains an integer n: the number of dams.
- The second line contains n integers: the flow rate of each dam.

## Output Format
- Return one integer: the total number of valid combinationss.

## Constraints
- 1 ≤ n ≤ 60
- 1 ≤ flow rate ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths, dynamic-programming
