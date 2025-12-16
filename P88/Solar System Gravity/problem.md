## Title
Solar System Gravity

## Slug
solar-system-gravity

## Difficulty
Medium

## Description
Planets have different masses. To destabilize an orbit, a planetary alignment must exert more than half the total gravitational pull of the system.

Your task is to count the number of **alignmentss**. A alignment is considered valid if it satisfies two specific criteria:
1.  **Orbit Shift:** The total mass of the alignment is strictly greater than half of the total mass across all planets.
2.  **No Superfluous planets:** The alignment is minimal. This means that removing **any one** planet from the alignment would cause the remaining total to drop to half or less of the total mass (losing the Orbit Shift).

## Examples

### 1

#### Input
5
3 1 4 1 5

#### Output
4

#### Explanation
Total mass is 14. Half is 7. We need a sum > 7.
The group {5, 4, 1} (Sum 10) is **not** valid because removing 1 leaves 9, which is still > 7.
Valid groups are those where every member is critical.

### 2

#### Input
4
1 2 3 4

#### Output
3

#### Explanation
Total mass = 10. Half = 5.
Valid alignmentss: {4, 2}, {4, 3}, {3, 2, 1}.

## Input Format
- The first line contains an integer n: the number of planets.
- The second line contains n integers: the mass of each planet.

## Output Format
- Return one integer: the total number of valid alignmentss.

## Constraints
- 1 ≤ n ≤ 60
- 1 ≤ mass ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths, dynamic-programming
