## Title
Email List Scrubbing

## Slug
email-list-scrubbing

## Difficulty
Easy

## Description
A marketing tool scrubs an email list. Duplicate email hashes are removed to save sending costs.

Your task is to determine if any email hash appears at least twice in the list.

## Examples

### 1

#### Input
4
1 2 3 1

#### Output
Yes

#### Explanation
The email hash `1` appears twice.

### 2

#### Input
4
1 2 3 4

#### Output
No

#### Explanation
All email hashs are distinct.

## Input Format
- The first line contains a single integer n, the number of subscribers.
- The second line contains n space-separated integers, representing the email hashs.

## Output Format
- Return `Yes` if any email hash appears at least twice, otherwise `No`.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ values ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
sorting, array, hash-table
