## Title
Virus Mutation

## Slug
virus-mutation

## Difficulty
Medium

## Description
Viral strains have different infection rates. A pandemic starts if a cluster of strains has a combined rate exceeding half the total potential infection rate.

Your task is to count the number of **clusterss**. A cluster is considered valid if it satisfies two specific criteria:
1.  **Pandemic:** The total infection rate of the cluster is strictly greater than half of the total infection rate across all strains.
2.  **No Superfluous strains:** The cluster is minimal. This means that removing **any one** strain from the cluster would cause the remaining total to drop to half or less of the total infection rate (losing the Pandemic).

## Examples

### 1

#### Input
5
3 1 4 1 5

#### Output
4

#### Explanation
Total infection rate is 14. Half is 7. We need a sum > 7.
The group {5, 4, 1} (Sum 10) is **not** valid because removing 1 leaves 9, which is still > 7.
Valid groups are those where every member is critical.

### 2

#### Input
4
1 2 3 4

#### Output
3

#### Explanation
Total infection rate = 10. Half = 5.
Valid clusterss: {4, 2}, {4, 3}, {3, 2, 1}.

## Input Format
- The first line contains an integer n: the number of strains.
- The second line contains n integers: the infection rate of each strain.

## Output Format
- Return one integer: the total number of valid clusterss.

## Constraints
- 1 ≤ n ≤ 60
- 1 ≤ infection rate ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths, dynamic-programming
