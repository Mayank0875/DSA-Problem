## Title
Chemical Reaction

## Slug
chemical-reaction

## Difficulty
Medium

## Description
Reagents have different molar concentrations. A reaction triggers only if the mixed reagents account for more than half the total moles available.

Your task is to count the number of **mixturess**. A mixture is considered valid if it satisfies two specific criteria:
1.  **Reaction Trigger:** The total concentration of the mixture is strictly greater than half of the total concentration across all reagents.
2.  **No Superfluous reagents:** The mixture is minimal. This means that removing **any one** reagent from the mixture would cause the remaining total to drop to half or less of the total concentration (losing the Reaction Trigger).

## Examples

### 1

#### Input
5
3 1 4 1 5

#### Output
4

#### Explanation
Total concentration is 14. Half is 7. We need a sum > 7.
The group {5, 4, 1} (Sum 10) is **not** valid because removing 1 leaves 9, which is still > 7.
Valid groups are those where every member is critical.

### 2

#### Input
4
1 2 3 4

#### Output
3

#### Explanation
Total concentration = 10. Half = 5.
Valid mixturess: {4, 2}, {4, 3}, {3, 2, 1}.

## Input Format
- The first line contains an integer n: the number of reagents.
- The second line contains n integers: the concentration of each reagent.

## Output Format
- Return one integer: the total number of valid mixturess.

## Constraints
- 1 ≤ n ≤ 60
- 1 ≤ concentration ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths, dynamic-programming
