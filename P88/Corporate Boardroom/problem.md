## Title
Corporate Boardroom

## Slug
corporate-boardroom

## Difficulty
Medium

## Description
A corporation has several shareholders, each owning a specific number of shares. To pass a resolution, a group of shareholders must hold a strict majority of the total shares.

Your task is to count the number of **voting blocss**. A voting bloc is considered valid if it satisfies two specific criteria:
1.  **Majority Control:** The total shares of the voting bloc is strictly greater than half of the total shares across all shareholders.
2.  **No Superfluous shareholders:** The voting bloc is minimal. This means that removing **any one** shareholder from the voting bloc would cause the remaining total to drop to half or less of the total shares (losing the Majority Control).

## Examples

### 1

#### Input
5
3 1 4 1 5

#### Output
4

#### Explanation
Total shares is 14. Half is 7. We need a sum > 7.
The group {5, 4, 1} (Sum 10) is **not** valid because removing 1 leaves 9, which is still > 7.
Valid groups are those where every member is critical.

### 2

#### Input
4
1 2 3 4

#### Output
3

#### Explanation
Total shares = 10. Half = 5.
Valid voting blocss: {4, 2}, {4, 3}, {3, 2, 1}.

## Input Format
- The first line contains an integer n: the number of shareholders.
- The second line contains n integers: the shares of each shareholder.

## Output Format
- Return one integer: the total number of valid voting blocss.

## Constraints
- 1 ≤ n ≤ 60
- 1 ≤ shares ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths, dynamic-programming
