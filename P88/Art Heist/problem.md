## Title
Art Heist

## Slug
art-heist

## Difficulty
Medium

## Description
Paintings have different black market values. A heist is considered legendary if the stolen set represents more than half the gallery's total value.

Your task is to count the number of **haulss**. A haul is considered valid if it satisfies two specific criteria:
1.  **Legendary Status:** The total value of the haul is strictly greater than half of the total value across all paintings.
2.  **No Superfluous paintings:** The haul is minimal. This means that removing **any one** painting from the haul would cause the remaining total to drop to half or less of the total value (losing the Legendary Status).

## Examples

### 1

#### Input
5
3 1 4 1 5

#### Output
4

#### Explanation
Total value is 14. Half is 7. We need a sum > 7.
The group {5, 4, 1} (Sum 10) is **not** valid because removing 1 leaves 9, which is still > 7.
Valid groups are those where every member is critical.

### 2

#### Input
4
1 2 3 4

#### Output
3

#### Explanation
Total value = 10. Half = 5.
Valid haulss: {4, 2}, {4, 3}, {3, 2, 1}.

## Input Format
- The first line contains an integer n: the number of paintings.
- The second line contains n integers: the value of each painting.

## Output Format
- Return one integer: the total number of valid haulss.

## Constraints
- 1 ≤ n ≤ 60
- 1 ≤ value ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths, dynamic-programming
