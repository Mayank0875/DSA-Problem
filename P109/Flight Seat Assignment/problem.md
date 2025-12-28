## Title
Flight Seat Assignment

## Slug
flight-seat-assignment

## Difficulty
Easy

## Description
An airline system checks the manifest. Two passengers assigned the same seat ID (hashed) is a critical error.

Your task is to determine if any seat ID appears at least twice in the list.

## Examples

### 1

#### Input
4
1 2 3 1

#### Output
Yes

#### Explanation
The seat ID `1` appears twice.

### 2

#### Input
4
1 2 3 4

#### Output
No

#### Explanation
All seat IDs are distinct.

## Input Format
- The first line contains a single integer n, the number of assignments.
- The second line contains n space-separated integers, representing the seat IDs.

## Output Format
- Return `Yes` if any seat ID appears at least twice, otherwise `No`.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ values ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
sorting, array, hash-table
