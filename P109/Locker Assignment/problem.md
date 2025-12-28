## Title
Locker Assignment

## Slug
locker-assignment

## Difficulty
Easy

## Description
A school assigns lockers to students. The admin checks the assignment list to ensure no locker number was assigned to multiple students.

Your task is to determine if any locker number appears at least twice in the list.

## Examples

### 1

#### Input
4
1 2 3 1

#### Output
Yes

#### Explanation
The locker number `1` appears twice.

### 2

#### Input
4
1 2 3 4

#### Output
No

#### Explanation
All locker numbers are distinct.

## Input Format
- The first line contains a single integer n, the number of assignments.
- The second line contains n space-separated integers, representing the locker numbers.

## Output Format
- Return `Yes` if any locker number appears at least twice, otherwise `No`.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ values ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
sorting, array, hash-table
