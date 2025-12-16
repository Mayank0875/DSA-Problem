## Title
Auction Bidding

## Slug
auction-bidding

## Difficulty
Medium

## Description
Bidders have different budget caps. To win a lot, a syndicate of bidders must pool a budget greater than half the total market capital.

Your task is to count the number of **syndicatess**. A syndicate is considered valid if it satisfies two specific criteria:
1.  **Winning Bid:** The total budget of the syndicate is strictly greater than half of the total budget across all bidders.
2.  **No Superfluous bidders:** The syndicate is minimal. This means that removing **any one** bidder from the syndicate would cause the remaining total to drop to half or less of the total budget (losing the Winning Bid).

## Examples

### 1

#### Input
5
3 1 4 1 5

#### Output
4

#### Explanation
Total budget is 14. Half is 7. We need a sum > 7.
The group {5, 4, 1} (Sum 10) is **not** valid because removing 1 leaves 9, which is still > 7.
Valid groups are those where every member is critical.

### 2

#### Input
4
1 2 3 4

#### Output
3

#### Explanation
Total budget = 10. Half = 5.
Valid syndicatess: {4, 2}, {4, 3}, {3, 2, 1}.

## Input Format
- The first line contains an integer n: the number of bidders.
- The second line contains n integers: the budget of each bidder.

## Output Format
- Return one integer: the total number of valid syndicatess.

## Constraints
- 1 ≤ n ≤ 60
- 1 ≤ budget ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths, dynamic-programming
