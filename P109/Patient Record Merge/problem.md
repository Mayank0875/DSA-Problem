## Title
Patient Record Merge

## Slug
patient-record-merge

## Difficulty
Easy

## Description
A hospital merges records from two departments. The system checks if any Patient ID appears more than once in the merged list.

Your task is to determine if any patient ID appears at least twice in the list.

## Examples

### 1

#### Input
4
1 2 3 1

#### Output
Yes

#### Explanation
The patient ID `1` appears twice.

### 2

#### Input
4
1 2 3 4

#### Output
No

#### Explanation
All patient IDs are distinct.

## Input Format
- The first line contains a single integer n, the number of records.
- The second line contains n space-separated integers, representing the patient IDs.

## Output Format
- Return `Yes` if any patient ID appears at least twice, otherwise `No`.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ values ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
sorting, array, hash-table
