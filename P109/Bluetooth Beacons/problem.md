## Title
Bluetooth Beacons

## Slug
bluetooth-beacons

## Difficulty
Easy

## Description
A store tracks Bluetooth beacons on carts. If the same beacon ID is detected in two different aisles simultaneously, it's an error.

Your task is to determine if any beacon ID appears at least twice in the list.

## Examples

### 1

#### Input
4
1 2 3 1

#### Output
Yes

#### Explanation
The beacon ID `1` appears twice.

### 2

#### Input
4
1 2 3 4

#### Output
No

#### Explanation
All beacon IDs are distinct.

## Input Format
- The first line contains a single integer n, the number of detections.
- The second line contains n space-separated integers, representing the beacon IDs.

## Output Format
- Return `Yes` if any beacon ID appears at least twice, otherwise `No`.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ values ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
sorting, array, hash-table
