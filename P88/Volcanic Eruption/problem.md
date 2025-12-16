## Title
Volcanic Eruption

## Slug
volcanic-eruption

## Difficulty
Medium

## Description
Vents release different amounts of pressure. An eruption occurs if a set of open vents releases more than half the total subterranean pressure.

Your task is to count the number of **vent setss**. A vent set is considered valid if it satisfies two specific criteria:
1.  **Eruption:** The total pressure of the vent set is strictly greater than half of the total pressure across all vents.
2.  **No Superfluous vents:** The vent set is minimal. This means that removing **any one** vent from the vent set would cause the remaining total to drop to half or less of the total pressure (losing the Eruption).

## Examples

### 1

#### Input
5
3 1 4 1 5

#### Output
4

#### Explanation
Total pressure is 14. Half is 7. We need a sum > 7.
The group {5, 4, 1} (Sum 10) is **not** valid because removing 1 leaves 9, which is still > 7.
Valid groups are those where every member is critical.

### 2

#### Input
4
1 2 3 4

#### Output
3

#### Explanation
Total pressure = 10. Half = 5.
Valid vent setss: {4, 2}, {4, 3}, {3, 2, 1}.

## Input Format
- The first line contains an integer n: the number of vents.
- The second line contains n integers: the pressure of each vent.

## Output Format
- Return one integer: the total number of valid vent setss.

## Constraints
- 1 ≤ n ≤ 60
- 1 ≤ pressure ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths, dynamic-programming
