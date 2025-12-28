## Title
Magic Spell Book

## Slug
magic-spell-book

## Difficulty
Easy

## Description
A wizard compiles a spellbook. Duplicate spell IDs (hashed from incantations) mean the wizard wrote the same spell twice.

Your task is to determine if any spell ID appears at least twice in the list.

## Examples

### 1

#### Input
4
1 2 3 1

#### Output
Yes

#### Explanation
The spell ID `1` appears twice.

### 2

#### Input
4
1 2 3 4

#### Output
No

#### Explanation
All spell IDs are distinct.

## Input Format
- The first line contains a single integer n, the number of pages.
- The second line contains n space-separated integers, representing the spell IDs.

## Output Format
- Return `Yes` if any spell ID appears at least twice, otherwise `No`.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ values ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
sorting, array, hash-table
