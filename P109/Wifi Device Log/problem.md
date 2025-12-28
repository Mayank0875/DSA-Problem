## Title
Wifi Device Log

## Slug
wifi-device-log

## Difficulty
Easy

## Description
A router logs connected MAC addresses (hashed to integers). Duplicate entries in the active client table indicate a display bug.

Your task is to determine if any MAC hash appears at least twice in the list.

## Examples

### 1

#### Input
4
1 2 3 1

#### Output
Yes

#### Explanation
The MAC hash `1` appears twice.

### 2

#### Input
4
1 2 3 4

#### Output
No

#### Explanation
All MAC hashs are distinct.

## Input Format
- The first line contains a single integer n, the number of devices.
- The second line contains n space-separated integers, representing the MAC hashs.

## Output Format
- Return `Yes` if any MAC hash appears at least twice, otherwise `No`.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ values ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
sorting, array, hash-table
