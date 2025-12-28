## Title
Social Security Audit

## Slug
social-security-audit

## Difficulty
Easy

## Description
A government agency checks a list of beneficiaries. Each person should appear only once based on their SSN hash.

Your task is to determine if any SSN hash appears at least twice in the list.

## Examples

### 1

#### Input
4
1 2 3 1

#### Output
Yes

#### Explanation
The SSN hash `1` appears twice.

### 2

#### Input
4
1 2 3 4

#### Output
No

#### Explanation
All SSN hashs are distinct.

## Input Format
- The first line contains a single integer n, the number of records.
- The second line contains n space-separated integers, representing the SSN hashs.

## Output Format
- Return `Yes` if any SSN hash appears at least twice, otherwise `No`.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ values ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
sorting, array, hash-table
