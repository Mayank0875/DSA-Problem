## Title
Server Request Log

## Slug
server-request-log

## Difficulty
Easy

## Description
A server tracks Request IDs to ensure idempotency. Processing the same Request ID twice could corrupt state.

Your task is to determine if any request ID appears at least twice in the list.

## Examples

### 1

#### Input
4
1 2 3 1

#### Output
Yes

#### Explanation
The request ID `1` appears twice.

### 2

#### Input
4
1 2 3 4

#### Output
No

#### Explanation
All request IDs are distinct.

## Input Format
- The first line contains a single integer n, the number of requests.
- The second line contains n space-separated integers, representing the request IDs.

## Output Format
- Return `Yes` if any request ID appears at least twice, otherwise `No`.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ values ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
sorting, array, hash-table
