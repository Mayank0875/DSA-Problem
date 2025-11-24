## Title
Virus Mutation Strain

## Slug
virus-mutation-strain

## Difficulty
Easy

## Description
Virologists sort virus strains by severity ID. Rare mutations appearing in the sample are isolated first. If mutation counts are equal, the strain with the higher severity is isolated first.

## Examples

### 1

#### Input
6
[1, 1, 2, 2, 2, 3]

#### Output
[3, 1, 1, 2, 2, 2]

#### Explanation
'3' has a frequency of 1, '1' has a frequency of 2, and '2' has a frequency of 3. They are sorted by increasing frequency.

### 2

#### Input
5
[2, 3, 1, 3, 2]

#### Output
[1, 3, 3, 2, 2]

#### Explanation
'1' has a frequency of 1. Both '2' and '3' have a frequency of 2. Since they have the same frequency, '3' is placed before '2' because it has a larger value.

## Input Format
- The first line contains a single integer n, representing the number of items.
- The second line contains n space-separated integers representing the item values.

## Output Format
- Return the sorted array of integers.

## Constraints
- 1 ≤ n ≤ 100
- -100 ≤ nums[i] ≤ 100

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, hash-table
