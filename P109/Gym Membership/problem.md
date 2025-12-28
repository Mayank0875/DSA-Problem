## Title
Gym Membership

## Slug
gym-membership

## Difficulty
Easy

## Description
A gym tracks active members entering the facility. Duplicate check-ins for the same member ID in a split second indicate a glitch.

Your task is to determine if any member ID appears at least twice in the list.

## Examples

### 1

#### Input
4
1 2 3 1

#### Output
Yes

#### Explanation
The member ID `1` appears twice.

### 2

#### Input
4
1 2 3 4

#### Output
No

#### Explanation
All member IDs are distinct.

## Input Format
- The first line contains a single integer n, the number of check-ins.
- The second line contains n space-separated integers, representing the member IDs.

## Output Format
- Return `Yes` if any member ID appears at least twice, otherwise `No`.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ values ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
sorting, array, hash-table
