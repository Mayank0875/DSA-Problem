## Title
Driver License Check

## Slug
driver-license-check

## Difficulty
Easy

## Description
A DMV database audit checks a list of active licenses. Duplicate license numbers are a sign of clerical error or fraud.

Your task is to determine if any license number appears at least twice in the list.

## Examples

### 1

#### Input
4
1 2 3 1

#### Output
Yes

#### Explanation
The license number `1` appears twice.

### 2

#### Input
4
1 2 3 4

#### Output
No

#### Explanation
All license numbers are distinct.

## Input Format
- The first line contains a single integer n, the number of licenses.
- The second line contains n space-separated integers, representing the license numbers.

## Output Format
- Return `Yes` if any license number appears at least twice, otherwise `No`.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ values ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
sorting, array, hash-table
