## Title
Meeting Participants

## Slug
meeting-participants

## Difficulty
Easy

## Description
A video conference tool checks the participant list. A user appearing twice usually means they joined from two devices.

Your task is to determine if any user ID appears at least twice in the list.

## Examples

### 1

#### Input
4
1 2 3 1

#### Output
Yes

#### Explanation
The user ID `1` appears twice.

### 2

#### Input
4
1 2 3 4

#### Output
No

#### Explanation
All user IDs are distinct.

## Input Format
- The first line contains a single integer n, the number of participants.
- The second line contains n space-separated integers, representing the user IDs.

## Output Format
- Return `Yes` if any user ID appears at least twice, otherwise `No`.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ values ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
sorting, array, hash-table
