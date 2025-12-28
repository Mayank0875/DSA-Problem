## Title
QR Code Tickets

## Slug
qr-code-tickets

## Difficulty
Easy

## Description
Event staff scan QR codes. The app must warn if a code has already been scanned to prevent entry fraud.

Your task is to determine if any QR hash appears at least twice in the list.

## Examples

### 1

#### Input
4
1 2 3 1

#### Output
Yes

#### Explanation
The QR hash `1` appears twice.

### 2

#### Input
4
1 2 3 4

#### Output
No

#### Explanation
All QR hashs are distinct.

## Input Format
- The first line contains a single integer n, the number of attendees.
- The second line contains n space-separated integers, representing the QR hashs.

## Output Format
- Return `Yes` if any QR hash appears at least twice, otherwise `No`.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ values ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
sorting, array, hash-table
