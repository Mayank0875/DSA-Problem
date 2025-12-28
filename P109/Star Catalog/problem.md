## Title
Star Catalog

## Slug
star-catalog

## Difficulty
Easy

## Description
Astronomers merge data from two telescopes. They check for duplicate star IDs to avoid double-counting celestial bodies.

Your task is to determine if any star ID appears at least twice in the list.

## Examples

### 1

#### Input
4
1 2 3 1

#### Output
Yes

#### Explanation
The star ID `1` appears twice.

### 2

#### Input
4
1 2 3 4

#### Output
No

#### Explanation
All star IDs are distinct.

## Input Format
- The first line contains a single integer n, the number of entries.
- The second line contains n space-separated integers, representing the star IDs.

## Output Format
- Return `Yes` if any star ID appears at least twice, otherwise `No`.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ values ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
sorting, array, hash-table
