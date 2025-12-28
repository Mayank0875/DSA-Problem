## Title
RFID Tag Scanner

## Slug
rfid-tag-scanner

## Difficulty
Easy

## Description
A retail gate scans items in a cart. Duplicate RFID tags in a single scan event might mean the reader is glitching.

Your task is to determine if any tag ID appears at least twice in the list.

## Examples

### 1

#### Input
4
1 2 3 1

#### Output
Yes

#### Explanation
The tag ID `1` appears twice.

### 2

#### Input
4
1 2 3 4

#### Output
No

#### Explanation
All tag IDs are distinct.

## Input Format
- The first line contains a single integer n, the number of items.
- The second line contains n space-separated integers, representing the tag IDs.

## Output Format
- Return `Yes` if any tag ID appears at least twice, otherwise `No`.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ values ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
sorting, array, hash-table
