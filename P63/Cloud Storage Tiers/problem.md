## Title
Cloud Storage Tiers

## Slug
cloud-storage-tiers

## Difficulty
Easy

## Description
A file is fragmented into $n$ parts. Each part is stored in one of 5 storage classes (Cold, Cool, Warm, Hot, Instant). For retrieval efficiency, the parts must be stored in non-decreasing order of access speed. How many storage configurations are possible?

## Examples

### 1

#### Input
1

#### Output
5

#### Explanation
There are 5 valid sequences of length 1.

### 2

#### Input
2

#### Output
15

#### Explanation
There are 15 valid sorted sequences of length 2 (e.g., aa, ae, ai, ao, au, ee, etc.).

## Input Format
- The input consists of a single integer n, representing the required length/quantity.

## Output Format
- Return a single integer representing the total number of valid sorted sequences.

## Constraints
- 1 ≤ n ≤ 50

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, math
