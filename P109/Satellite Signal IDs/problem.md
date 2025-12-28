## Title
Satellite Signal IDs

## Slug
satellite-signal-ids

## Difficulty
Easy

## Description
A ground station receives signals from a constellation. Duplicate signal IDs indicate a malfunction in a satellite.

Your task is to determine if any signal ID appears at least twice in the list.

## Examples

### 1

#### Input
4
1 2 3 1

#### Output
Yes

#### Explanation
The signal ID `1` appears twice.

### 2

#### Input
4
1 2 3 4

#### Output
No

#### Explanation
All signal IDs are distinct.

## Input Format
- The first line contains a single integer n, the number of signals.
- The second line contains n space-separated integers, representing the signal IDs.

## Output Format
- Return `Yes` if any signal ID appears at least twice, otherwise `No`.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ values ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
sorting, array, hash-table
