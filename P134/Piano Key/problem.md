## Title
Piano Key

## Slug
piano-key

## Difficulty
Medium

## Description
A piano has keys numbered 1 to 88. A MIDI file logs keys pressed. Find the lowest key number that is never used in the piece.

You are given an unsorted integer array `ids` representing the Key Numbers currently in the system. Some Key Numbers may be negative or zero (representing invalid or placeholder entries).

Your task is to find the **smallest positive** Key Number that is **missing** from the list. This will be the unused key.

**Note:** You must implement an algorithm that runs in $O(n)$ time and uses $O(1)$ auxiliary space.

## Examples

### 1

#### Input
3
1 2 0

#### Output
3

#### Explanation
The Key Numbers 1 and 2 are present. The smallest missing positive Key Number is 3.

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
- Return a single integer representing the smallest missing positive Key Number.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ ids[i] ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, hash-table

