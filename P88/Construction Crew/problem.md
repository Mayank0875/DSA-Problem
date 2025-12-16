## Title
Construction Crew

## Slug
construction-crew

## Difficulty
Medium

## Description
Workers have different lifting capacities. To lift a heavy beam, a team needs more than half the total lifting capacity of the entire crew.

Your task is to count the number of **teamss**. A team is considered valid if it satisfies two specific criteria:
1.  **Lift Success:** The total lifting capacity of the team is strictly greater than half of the total lifting capacity across all workers.
2.  **No Superfluous workers:** The team is minimal. This means that removing **any one** worker from the team would cause the remaining total to drop to half or less of the total lifting capacity (losing the Lift Success).

## Examples

### 1

#### Input
5
3 1 4 1 5

#### Output
4

#### Explanation
Total lifting capacity is 14. Half is 7. We need a sum > 7.
The group {5, 4, 1} (Sum 10) is **not** valid because removing 1 leaves 9, which is still > 7.
Valid groups are those where every member is critical.

### 2

#### Input
4
1 2 3 4

#### Output
3

#### Explanation
Total lifting capacity = 10. Half = 5.
Valid teamss: {4, 2}, {4, 3}, {3, 2, 1}.

## Input Format
- The first line contains an integer n: the number of workers.
- The second line contains n integers: the lifting capacity of each worker.

## Output Format
- Return one integer: the total number of valid teamss.

## Constraints
- 1 ≤ n ≤ 60
- 1 ≤ lifting capacity ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths, dynamic-programming
