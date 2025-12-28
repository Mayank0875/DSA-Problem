## Title
Exam Candidate List

## Slug
exam-candidate-list

## Difficulty
Easy

## Description
An exam center verifies the list of registered candidates. Duplicate candidate IDs mean a student registered twice.

Your task is to determine if any candidate ID appears at least twice in the list.

## Examples

### 1

#### Input
4
1 2 3 1

#### Output
Yes

#### Explanation
The candidate ID `1` appears twice.

### 2

#### Input
4
1 2 3 4

#### Output
No

#### Explanation
All candidate IDs are distinct.

## Input Format
- The first line contains a single integer n, the number of registrations.
- The second line contains n space-separated integers, representing the candidate IDs.

## Output Format
- Return `Yes` if any candidate ID appears at least twice, otherwise `No`.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ values ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
sorting, array, hash-table
