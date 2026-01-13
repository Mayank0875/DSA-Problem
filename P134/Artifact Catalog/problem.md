## Title
Artifact Catalog

## Slug
artifact-catalog

## Difficulty
Medium

## Description
A museum catalogs items with IDs starting at 1. The digital record is scrambled. Find the first ID that has not been assigned to an artifact yet.

You are given an unsorted integer array `ids` representing the Artifact IDs currently in the system. Some Artifact IDs may be negative or zero (representing invalid or placeholder entries).

Your task is to find the **smallest positive** Artifact ID that is **missing** from the list. This will be the next ID to assign.

**Note:** You must implement an algorithm that runs in $O(n)$ time and uses $O(1)$ auxiliary space.

## Examples

### 1

#### Input
3
1 2 0

#### Output
3

#### Explanation
The Artifact IDs 1 and 2 are present. The smallest missing positive Artifact ID is 3.

### 2

#### Input
4
3 4 -1 1

#### Output
2

#### Explanation
1 is present, but 2 is missing.

## Input Format
- The first line contains an integer $n$, the size of the array.
- The second line contains $n$ space-separated integers `ids`.

## Output Format
- Return a single integer representing the smallest missing positive Artifact ID.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ ids[i] ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, hash-table

