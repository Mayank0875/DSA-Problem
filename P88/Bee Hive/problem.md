## Title
Bee Hive

## Slug
bee-hive

## Difficulty
Medium

## Description
Bees collect different amounts of nectar. A swarm leaves to build a new hive if a group collecting more than half the nectar decides to leave.

Your task is to count the number of **swarmss**. A swarm is considered valid if it satisfies two specific criteria:
1.  **Swarm Decision:** The total nectar amount of the swarm is strictly greater than half of the total nectar amount across all bees.
2.  **No Superfluous bees:** The swarm is minimal. This means that removing **any one** bee from the swarm would cause the remaining total to drop to half or less of the total nectar amount (losing the Swarm Decision).

## Examples

### 1

#### Input
5
3 1 4 1 5

#### Output
4

#### Explanation
Total nectar amount is 14. Half is 7. We need a sum > 7.
The group {5, 4, 1} (Sum 10) is **not** valid because removing 1 leaves 9, which is still > 7.
Valid groups are those where every member is critical.

### 2

#### Input
4
1 2 3 4

#### Output
3

#### Explanation
Total nectar amount = 10. Half = 5.
Valid swarmss: {4, 2}, {4, 3}, {3, 2, 1}.

## Input Format
- The first line contains an integer n: the number of bees.
- The second line contains n integers: the nectar amount of each bee.

## Output Format
- Return one integer: the total number of valid swarmss.

## Constraints
- 1 ≤ n ≤ 60
- 1 ≤ nectar amount ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths, dynamic-programming
