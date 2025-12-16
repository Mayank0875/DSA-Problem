## Title
Cloud Computing

## Slug
cloud-computing

## Difficulty
Medium

## Description
A cluster of compute nodes has varying processing power (FLOPS). To handle a massive job, a sub-cluster needs more than half the total processing power of the entire data center.

Your task is to count the number of **sub-clusterss**. A sub-cluster is considered valid if it satisfies two specific criteria:
1.  **Compute Dominance:** The total processing power of the sub-cluster is strictly greater than half of the total processing power across all nodes.
2.  **No Superfluous nodes:** The sub-cluster is minimal. This means that removing **any one** node from the sub-cluster would cause the remaining total to drop to half or less of the total processing power (losing the Compute Dominance).

## Examples

### 1

#### Input
5
3 1 4 1 5

#### Output
4

#### Explanation
Total processing power is 14. Half is 7. We need a sum > 7.
The group {5, 4, 1} (Sum 10) is **not** valid because removing 1 leaves 9, which is still > 7.
Valid groups are those where every member is critical.

### 2

#### Input
4
1 2 3 4

#### Output
3

#### Explanation
Total processing power = 10. Half = 5.
Valid sub-clusterss: {4, 2}, {4, 3}, {3, 2, 1}.

## Input Format
- The first line contains an integer n: the number of nodes.
- The second line contains n integers: the processing power of each node.

## Output Format
- Return one integer: the total number of valid sub-clusterss.

## Constraints
- 1 ≤ n ≤ 60
- 1 ≤ processing power ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths, dynamic-programming
