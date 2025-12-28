## Title
Fingerprint Database

## Slug
fingerprint-database

## Difficulty
Easy

## Description
A biometric system imports user data. Duplicate fingerprint hashes imply a collision or data duplication.

Your task is to determine if any fingerprint hash appears at least twice in the list.

## Examples

### 1

#### Input
4
1 2 3 1

#### Output
Yes

#### Explanation
The fingerprint hash `1` appears twice.

### 2

#### Input
4
1 2 3 4

#### Output
No

#### Explanation
All fingerprint hashs are distinct.

## Input Format
- The first line contains a single integer n, the number of users.
- The second line contains n space-separated integers, representing the fingerprint hashs.

## Output Format
- Return `Yes` if any fingerprint hash appears at least twice, otherwise `No`.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ values ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
sorting, array, hash-table
