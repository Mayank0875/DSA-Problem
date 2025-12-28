## Title
Lottery Ticket Validation

## Slug
lottery-ticket-validation

## Difficulty
Easy

## Description
A lottery system prints tickets with unique serial numbers. A glitch may have caused duplicates. You need to check the batch of printed tickets.

Your task is to determine if any serial number appears at least twice in the list.

## Examples

### 1

#### Input
4
1 2 3 1

#### Output
Yes

#### Explanation
The serial number `1` appears twice.

### 2

#### Input
4
1 2 3 4

#### Output
No

#### Explanation
All serial numbers are distinct.

## Input Format
- The first line contains a single integer n, the number of tickets.
- The second line contains n space-separated integers, representing the serial numbers.

## Output Format
- Return `Yes` if any serial number appears at least twice, otherwise `No`.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ values ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
sorting, array, hash-table
