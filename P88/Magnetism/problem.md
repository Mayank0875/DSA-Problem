## Title
Magnetism

## Slug
magnetism

## Difficulty
Medium

## Description
Magnets have different field strengths. To flip the polarity of a core, a cluster of magnets must exert more than half the total magnetic force.

Your task is to count the number of **clusterss**. A cluster is considered valid if it satisfies two specific criteria:
1.  **Polarity Flip:** The total field strength of the cluster is strictly greater than half of the total field strength across all magnets.
2.  **No Superfluous magnets:** The cluster is minimal. This means that removing **any one** magnet from the cluster would cause the remaining total to drop to half or less of the total field strength (losing the Polarity Flip).

## Examples

### 1

#### Input
5
3 1 4 1 5

#### Output
4

#### Explanation
Total field strength is 14. Half is 7. We need a sum > 7.
The group {5, 4, 1} (Sum 10) is **not** valid because removing 1 leaves 9, which is still > 7.
Valid groups are those where every member is critical.

### 2

#### Input
4
1 2 3 4

#### Output
3

#### Explanation
Total field strength = 10. Half = 5.
Valid clusterss: {4, 2}, {4, 3}, {3, 2, 1}.

## Input Format
- The first line contains an integer n: the number of magnets.
- The second line contains n integers: the field strength of each magnet.

## Output Format
- Return one integer: the total number of valid clusterss.

## Constraints
- 1 ≤ n ≤ 60
- 1 ≤ field strength ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths, dynamic-programming
