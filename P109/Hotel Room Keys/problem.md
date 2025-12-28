## Title
Hotel Room Keys

## Slug
hotel-room-keys

## Difficulty
Easy

## Description
A hotel key card system assigns IDs to active cards. Duplicate active IDs for different guests would be a security breach.

Your task is to determine if any key card ID appears at least twice in the list.

## Examples

### 1

#### Input
4
1 2 3 1

#### Output
Yes

#### Explanation
The key card ID `1` appears twice.

### 2

#### Input
4
1 2 3 4

#### Output
No

#### Explanation
All key card IDs are distinct.

## Input Format
- The first line contains a single integer n, the number of active keys.
- The second line contains n space-separated integers, representing the key card IDs.

## Output Format
- Return `Yes` if any key card ID appears at least twice, otherwise `No`.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ values ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
sorting, array, hash-table
