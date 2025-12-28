## Title
Parking Enforcement

## Slug
parking-enforcement

## Difficulty
Easy

## Description
A camera scans license plates entering a garage. If the same plate is logged twice without an exit, something is wrong.

Your task is to determine if any plate hash appears at least twice in the list.

## Examples

### 1

#### Input
4
1 2 3 1

#### Output
Yes

#### Explanation
The plate hash `1` appears twice.

### 2

#### Input
4
1 2 3 4

#### Output
No

#### Explanation
All plate hashs are distinct.

## Input Format
- The first line contains a single integer n, the number of entries.
- The second line contains n space-separated integers, representing the plate hashs.

## Output Format
- Return `Yes` if any plate hash appears at least twice, otherwise `No`.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ values ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
sorting, array, hash-table
