## Title
Concert Ticket Scan

## Slug
concert-ticket-scan

## Difficulty
Easy

## Description
Ushers scan tickets at a concert. If a ticket ID is scanned that has already been entered, it is a duplicate or fake.

Your task is to determine if any ticket ID appears at least twice in the list.

## Examples

### 1

#### Input
4
1 2 3 1

#### Output
Yes

#### Explanation
The ticket ID `1` appears twice.

### 2

#### Input
4
1 2 3 4

#### Output
No

#### Explanation
All ticket IDs are distinct.

## Input Format
- The first line contains a single integer n, the number of scans.
- The second line contains n space-separated integers, representing the ticket IDs.

## Output Format
- Return `Yes` if any ticket ID appears at least twice, otherwise `No`.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ values ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
sorting, array, hash-table
