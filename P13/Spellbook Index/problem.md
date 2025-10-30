## Title

Spellbook Index

## Slug

spellbook-index

## Difficulty

Easy

## Description

A wizard's spellbook is indexed by a sorted list of spell IDs. To cast a spell, the wizard must first find its ID in the index. Your task is to write a function that takes the sorted list of spell IDs and a `target` ID. The function should efficiently find whether the spell is in the book. You must write an algorithm with O(log n) runtime complexity.

## Examples

### 1

#### Input

6 8
[2, 5, 7, 8, 11, 12]


#### Output

1

#### Explanation

The target ID 8 is found in the list of grimoire IDs.

### 2

#### Input

6 6
[2, 5, 7, 8, 11, 12]

#### Output

0

#### Explanation

The target ID 6 is not found in the list.

## Input Format

- The first line contains an integers n and target , the number of grimoires and the ID of the grimoire to find. 
- The second line contains n space-separated integers representing the sorted grimoire IDs.

## Output Format

- Return 1 if the target is found, and 0 otherwise.

## Constraints

- 1 ≤ n ≤ 10^5
- 1 ≤ grimoire_id, target ≤ 10^9
- The grimoire IDs are sorted in non-decreasing order.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

binary-search, array, searching