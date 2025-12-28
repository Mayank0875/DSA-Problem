## Title
Contact List Cleanup

## Slug
contact-list-cleanup

## Difficulty
Easy

## Description
A phonebook app is importing contacts. It needs to check if there are duplicate phone numbers in the import list.

Your task is to determine if any phone number appears at least twice in the list.

## Examples

### 1

#### Input
4
1 2 3 1

#### Output
Yes

#### Explanation
The phone number `1` appears twice.

### 2

#### Input
4
1 2 3 4

#### Output
No

#### Explanation
All phone numbers are distinct.

## Input Format
- The first line contains a single integer n, the number of contacts.
- The second line contains n space-separated integers, representing the phone numbers.

## Output Format
- Return `Yes` if any phone number appears at least twice, otherwise `No`.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ values ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
sorting, array, hash-table
