## Title
Product Serial Numbers

## Slug
product-serial-numbers

## Difficulty
Easy

## Description
A manufacturer checks a batch of electronics. Duplicate serial numbers mean a printing error on the assembly line.

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
- The first line contains a single integer n, the number of products.
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
