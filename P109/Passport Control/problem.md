## Title
Passport Control

## Slug
passport-control

## Difficulty
Easy

## Description
At an airport gate, passengers scan their passports. The system must alert security if the same passport number has been scanned multiple times for the same flight.

Your task is to determine if any passport number appears at least twice in the list.

## Examples

### 1

#### Input
4
1 2 3 1

#### Output
Yes

#### Explanation
The passport number `1` appears twice.

### 2

#### Input
4
1 2 3 4

#### Output
No

#### Explanation
All passport numbers are distinct.

## Input Format
- The first line contains a single integer n, the number of scans.
- The second line contains n space-separated integers, representing the passport numbers.

## Output Format
- Return `Yes` if any passport number appears at least twice, otherwise `No`.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ values ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
sorting, array, hash-table
