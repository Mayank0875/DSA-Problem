## Title
Ant Colony

## Slug
ant-colony

## Difficulty
Medium

## Description
Ant groups carry different pheromone intensities. To trigger a migration, a group of ants must emit pheromones exceeding half the colony's total capacity.

Your task is to count the number of **signalss**. A signal is considered valid if it satisfies two specific criteria:
1.  **Migration Trigger:** The total pheromone level of the signal is strictly greater than half of the total pheromone level across all ants.
2.  **No Superfluous ants:** The signal is minimal. This means that removing **any one** ant from the signal would cause the remaining total to drop to half or less of the total pheromone level (losing the Migration Trigger).

## Examples

### 1

#### Input
5
3 1 4 1 5

#### Output
4

#### Explanation
Total pheromone level is 14. Half is 7. We need a sum > 7.
The group {5, 4, 1} (Sum 10) is **not** valid because removing 1 leaves 9, which is still > 7.
Valid groups are those where every member is critical.

### 2

#### Input
4
1 2 3 4

#### Output
3

#### Explanation
Total pheromone level = 10. Half = 5.
Valid signalss: {4, 2}, {4, 3}, {3, 2, 1}.

## Input Format
- The first line contains an integer n: the number of ants.
- The second line contains n integers: the pheromone level of each ant.

## Output Format
- Return one integer: the total number of valid signalss.

## Constraints
- 1 ≤ n ≤ 60
- 1 ≤ pheromone level ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths, dynamic-programming
