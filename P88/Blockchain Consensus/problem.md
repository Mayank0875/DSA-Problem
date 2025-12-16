## Title
Blockchain Consensus

## Slug
blockchain-consensus

## Difficulty
Medium

## Description
Validators in a Proof-of-Stake network have different amounts of staked tokens. To validate a block, a group must hold a majority of the total staked tokens.

Your task is to count the number of **consensus groupss**. A consensus group is considered valid if it satisfies two specific criteria:
1.  **51% Attack Potential:** The total stake of the consensus group is strictly greater than half of the total stake across all validators.
2.  **No Superfluous validators:** The consensus group is minimal. This means that removing **any one** validator from the consensus group would cause the remaining total to drop to half or less of the total stake (losing the 51% Attack Potential).

## Examples

### 1

#### Input
5
3 1 4 1 5

#### Output
4

#### Explanation
Total stake is 14. Half is 7. We need a sum > 7.
The group {5, 4, 1} (Sum 10) is **not** valid because removing 1 leaves 9, which is still > 7.
Valid groups are those where every member is critical.

### 2

#### Input
4
1 2 3 4

#### Output
3

#### Explanation
Total stake = 10. Half = 5.
Valid consensus groupss: {4, 2}, {4, 3}, {3, 2, 1}.

## Input Format
- The first line contains an integer n: the number of validators.
- The second line contains n integers: the stake of each validator.

## Output Format
- Return one integer: the total number of valid consensus groupss.

## Constraints
- 1 ≤ n ≤ 60
- 1 ≤ stake ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths, dynamic-programming
