## Title
Bus Ticket Validator

## Slug
bus-ticket-validator

## Difficulty
Easy

## Description
A bus scanner reads ticket codes. If the same daily pass code is used twice on the same trip, it's flagged.

Your task is to determine if any ticket code appears at least twice in the list.

## Examples

### 1

#### Input
4
1 2 3 1

#### Output
Yes

#### Explanation
The ticket code `1` appears twice.

### 2

#### Input
4
1 2 3 4

#### Output
No

#### Explanation
All ticket codes are distinct.

## Input Format
- The first line contains a single integer n, the number of passengers.
- The second line contains n space-separated integers, representing the ticket codes.

## Output Format
- Return `Yes` if any ticket code appears at least twice, otherwise `No`.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ values ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
sorting, array, hash-table
