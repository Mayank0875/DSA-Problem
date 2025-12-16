## Title
Orchestra Volume

## Slug
orchestra-volume

## Difficulty
Medium

## Description
Instruments produce different decibel levels. To reach a 'fortissimo' climax, a section of the orchestra must produce more than half the total possible volume.

Your task is to count the number of **sectionss**. A section is considered valid if it satisfies two specific criteria:
1.  **Fortissimo:** The total volume of the section is strictly greater than half of the total volume across all instruments.
2.  **No Superfluous instruments:** The section is minimal. This means that removing **any one** instrument from the section would cause the remaining total to drop to half or less of the total volume (losing the Fortissimo).

## Examples

### 1

#### Input
5
3 1 4 1 5

#### Output
4

#### Explanation
Total volume is 14. Half is 7. We need a sum > 7.
The group {5, 4, 1} (Sum 10) is **not** valid because removing 1 leaves 9, which is still > 7.
Valid groups are those where every member is critical.

### 2

#### Input
4
1 2 3 4

#### Output
3

#### Explanation
Total volume = 10. Half = 5.
Valid sectionss: {4, 2}, {4, 3}, {3, 2, 1}.

## Input Format
- The first line contains an integer n: the number of instruments.
- The second line contains n integers: the volume of each instrument.

## Output Format
- Return one integer: the total number of valid sectionss.

## Constraints
- 1 ≤ n ≤ 60
- 1 ≤ volume ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths, dynamic-programming
