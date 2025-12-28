## Title
Classroom Attendance

## Slug
classroom-attendance

## Difficulty
Easy

## Description
A digital attendance system logs student IDs as they enter. If a student ID is logged twice, the system needs to flag the anomaly.

Your task is to determine if any student ID appears at least twice in the list.

## Examples

### 1

#### Input
4
1 2 3 1

#### Output
Yes

#### Explanation
The student ID `1` appears twice.

### 2

#### Input
4
1 2 3 4

#### Output
No

#### Explanation
All student IDs are distinct.

## Input Format
- The first line contains a single integer n, the number of entries.
- The second line contains n space-separated integers, representing the student IDs.

## Output Format
- Return `Yes` if any student ID appears at least twice, otherwise `No`.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ values ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
sorting, array, hash-table
