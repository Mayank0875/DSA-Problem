## Title
Employee Badge Swipe

## Slug
employee-badge-swipe

## Difficulty
Easy

## Description
Security logs show badge swipes at a secure door. An employee shouldn't swipe in twice consecutively without swiping out.

Your task is to determine if any badge ID appears at least twice in the list.

## Examples

### 1

#### Input
4
1 2 3 1

#### Output
Yes

#### Explanation
The badge ID `1` appears twice.

### 2

#### Input
4
1 2 3 4

#### Output
No

#### Explanation
All badge IDs are distinct.

## Input Format
- The first line contains a single integer n, the number of swipes.
- The second line contains n space-separated integers, representing the badge IDs.

## Output Format
- Return `Yes` if any badge ID appears at least twice, otherwise `No`.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ values ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
sorting, array, hash-table
