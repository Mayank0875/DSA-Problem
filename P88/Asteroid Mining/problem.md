## Title
Asteroid Mining

## Slug
asteroid-mining

## Difficulty
Medium

## Description
Mining drones have different extraction rates. To deplete an asteroid quickly, a squad must have a combined rate greater than half the total fleet's rate.

Your task is to count the number of **squadss**. A squad is considered valid if it satisfies two specific criteria:
1.  **Rapid Depletion:** The total extraction rate of the squad is strictly greater than half of the total extraction rate across all drones.
2.  **No Superfluous drones:** The squad is minimal. This means that removing **any one** drone from the squad would cause the remaining total to drop to half or less of the total extraction rate (losing the Rapid Depletion).

## Examples

### 1

#### Input
5
3 1 4 1 5

#### Output
4

#### Explanation
Total extraction rate is 14. Half is 7. We need a sum > 7.
The group {5, 4, 1} (Sum 10) is **not** valid because removing 1 leaves 9, which is still > 7.
Valid groups are those where every member is critical.

### 2

#### Input
4
1 2 3 4

#### Output
3

#### Explanation
Total extraction rate = 10. Half = 5.
Valid squadss: {4, 2}, {4, 3}, {3, 2, 1}.

## Input Format
- The first line contains an integer n: the number of drones.
- The second line contains n integers: the extraction rate of each drone.

## Output Format
- Return one integer: the total number of valid squadss.

## Constraints
- 1 ≤ n ≤ 60
- 1 ≤ extraction rate ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths, dynamic-programming
