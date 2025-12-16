## Title
Ecological Balance

## Slug
ecological-balance

## Difficulty
Medium

## Description
Species in an ecosystem have different biomass. Ideally, a dominant group of species controls more than half the total biomass.

Your task is to count the number of **dominant groupss**. A dominant group is considered valid if it satisfies two specific criteria:
1.  **Dominance:** The total biomass of the dominant group is strictly greater than half of the total biomass across all species.
2.  **No Superfluous species:** The dominant group is minimal. This means that removing **any one** species from the dominant group would cause the remaining total to drop to half or less of the total biomass (losing the Dominance).

## Examples

### 1

#### Input
5
3 1 4 1 5

#### Output
4

#### Explanation
Total biomass is 14. Half is 7. We need a sum > 7.
The group {5, 4, 1} (Sum 10) is **not** valid because removing 1 leaves 9, which is still > 7.
Valid groups are those where every member is critical.

### 2

#### Input
4
1 2 3 4

#### Output
3

#### Explanation
Total biomass = 10. Half = 5.
Valid dominant groupss: {4, 2}, {4, 3}, {3, 2, 1}.

## Input Format
- The first line contains an integer n: the number of species.
- The second line contains n integers: the biomass of each species.

## Output Format
- Return one integer: the total number of valid dominant groupss.

## Constraints
- 1 ≤ n ≤ 60
- 1 ≤ biomass ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths, dynamic-programming
