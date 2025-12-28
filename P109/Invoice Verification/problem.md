## Title
Invoice Verification

## Slug
invoice-verification

## Difficulty
Easy

## Description
An accounting bot scans received invoices. It checks for duplicate invoice numbers from the same vendor to prevent double payment.

Your task is to determine if any invoice number appears at least twice in the list.

## Examples

### 1

#### Input
4
1 2 3 1

#### Output
Yes

#### Explanation
The invoice number `1` appears twice.

### 2

#### Input
4
1 2 3 4

#### Output
No

#### Explanation
All invoice numbers are distinct.

## Input Format
- The first line contains a single integer n, the number of invoices.
- The second line contains n space-separated integers, representing the invoice numbers.

## Output Format
- Return `Yes` if any invoice number appears at least twice, otherwise `No`.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ values ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
sorting, array, hash-table
