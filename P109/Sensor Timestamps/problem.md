## Title
Sensor Timestamps

## Slug
sensor-timestamps

## Difficulty
Easy

## Description
A data logger records readings. Duplicate timestamp IDs suggest the sensor is stuck or transmitting old data.

Your task is to determine if any timestamp appears at least twice in the list.

## Examples

### 1

#### Input
4
1 2 3 1

#### Output
Yes

#### Explanation
The timestamp `1` appears twice.

### 2

#### Input
4
1 2 3 4

#### Output
No

#### Explanation
All timestamps are distinct.

## Input Format
- The first line contains a single integer n, the number of readings.
- The second line contains n space-separated integers, representing the timestamps.

## Output Format
- Return `Yes` if any timestamp appears at least twice, otherwise `No`.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ values ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
sorting, array, hash-table
