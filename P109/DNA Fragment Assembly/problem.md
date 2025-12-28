## Title
DNA Fragment Assembly

## Slug
dna-fragment-assembly

## Difficulty
Easy

## Description
A sequencer reads DNA fragments. Duplicate fragment IDs indicate a reading error in the sequencing machine.

Your task is to determine if any fragment ID appears at least twice in the list.

## Examples

### 1

#### Input
4
1 2 3 1

#### Output
Yes

#### Explanation
The fragment ID `1` appears twice.

### 2

#### Input
4
1 2 3 4

#### Output
No

#### Explanation
All fragment IDs are distinct.

## Input Format
- The first line contains a single integer n, the number of reads.
- The second line contains n space-separated integers, representing the fragment IDs.

## Output Format
- Return `Yes` if any fragment ID appears at least twice, otherwise `No`.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ values ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
sorting, array, hash-table
