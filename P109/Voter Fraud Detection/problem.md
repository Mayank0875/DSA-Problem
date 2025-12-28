## Title
Voter Fraud Detection

## Slug
voter-fraud-detection

## Difficulty
Easy

## Description
An election commission is verifying votes. Each voter has a unique ID. If an ID appears more than once in the ballot box, it indicates potential double voting.

Your task is to determine if any voter ID appears at least twice in the list.

## Examples

### 1

#### Input
4
1 2 3 1

#### Output
Yes

#### Explanation
The voter ID `1` appears twice.

### 2

#### Input
4
1 2 3 4

#### Output
No

#### Explanation
All voter IDs are distinct.

## Input Format
- The first line contains a single integer n, the number of votes.
- The second line contains n space-separated integers, representing the voter IDs.

## Output Format
- Return `Yes` if any voter ID appears at least twice, otherwise `No`.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ values ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
sorting, array, hash-table
