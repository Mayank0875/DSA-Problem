## Title
Event Log Audit

## Slug
event-log-audit

## Difficulty
Easy

## Description
A security auditor checks system logs. Duplicate Event IDs are a sign of log tampering or buffering errors.

Your task is to determine if any event ID appears at least twice in the list.

## Examples

### 1

#### Input
4
1 2 3 1

#### Output
Yes

#### Explanation
The event ID `1` appears twice.

### 2

#### Input
4
1 2 3 4

#### Output
No

#### Explanation
All event IDs are distinct.

## Input Format
- The first line contains a single integer n, the number of logs.
- The second line contains n space-separated integers, representing the event IDs.

## Output Format
- Return `Yes` if any event ID appears at least twice, otherwise `No`.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ values ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
sorting, array, hash-table
