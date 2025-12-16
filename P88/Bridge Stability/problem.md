## Title
Bridge Stability

## Slug
bridge-stability

## Difficulty
Medium

## Description
A bridge is supported by pillars with different load-bearing capacities. If a set of pillars fails, the bridge collapses. We are looking for sets of pillars that carry the *majority* of the load capability.

Your task is to count the number of **support setss**. A support set is considered valid if it satisfies two specific criteria:
1.  **Primary Support:** The total load capacity of the support set is strictly greater than half of the total load capacity across all pillars.
2.  **No Superfluous pillars:** The support set is minimal. This means that removing **any one** pillar from the support set would cause the remaining total to drop to half or less of the total load capacity (losing the Primary Support).

## Examples

### 1

#### Input
5
3 1 4 1 5

#### Output
4

#### Explanation
Total load capacity is 14. Half is 7. We need a sum > 7.
The group {5, 4, 1} (Sum 10) is **not** valid because removing 1 leaves 9, which is still > 7.
Valid groups are those where every member is critical.

### 2

#### Input
4
1 2 3 4

#### Output
3

#### Explanation
Total load capacity = 10. Half = 5.
Valid support setss: {4, 2}, {4, 3}, {3, 2, 1}.

## Input Format
- The first line contains an integer n: the number of pillars.
- The second line contains n integers: the load capacity of each pillar.

## Output Format
- Return one integer: the total number of valid support setss.

## Constraints
- 1 ≤ n ≤ 60
- 1 ≤ load capacity ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths, dynamic-programming
