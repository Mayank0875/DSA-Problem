## Title
Survey Responses

## Slug
survey-responses

## Difficulty
Easy

## Description
A survey platform filters spam. Multiple submissions from the same Respondent ID need to be identified.

Your task is to determine if any respondent ID appears at least twice in the list.

## Examples

### 1

#### Input
4
1 2 3 1

#### Output
Yes

#### Explanation
The respondent ID `1` appears twice.

### 2

#### Input
4
1 2 3 4

#### Output
No

#### Explanation
All respondent IDs are distinct.

## Input Format
- The first line contains a single integer n, the number of submissions.
- The second line contains n space-separated integers, representing the respondent IDs.

## Output Format
- Return `Yes` if any respondent ID appears at least twice, otherwise `No`.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ values ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
sorting, array, hash-table
