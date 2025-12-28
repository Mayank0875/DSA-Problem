## Title
Username Registration

## Slug
username-registration

## Difficulty
Easy

## Description
A new social network checks requested usernames. If a requested username ID already exists in the database, it rejects the request.

Your task is to determine if any username ID appears at least twice in the list.

## Examples

### 1

#### Input
4
1 2 3 1

#### Output
Yes

#### Explanation
The username ID `1` appears twice.

### 2

#### Input
4
1 2 3 4

#### Output
No

#### Explanation
All username IDs are distinct.

## Input Format
- The first line contains a single integer n, the number of requests.
- The second line contains n space-separated integers, representing the username IDs.

## Output Format
- Return `Yes` if any username ID appears at least twice, otherwise `No`.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ values ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
sorting, array, hash-table
