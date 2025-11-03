## Title

Wizard's Rotated Scroll

## Slug

wizards-rotated-scroll

## Difficulty

Medium

## Description

A wizard's ancient scroll contains runes sorted by power level (a unique number). The scroll is circular, and the wizard started reading from an unknown point, creating a "rotated" sequence. For example, runes [10, 20, 30, 40] might be read as [30, 40, 10, 20]. You are given this sequence of power levels and a target level to find. Determine the position (index) of the target rune. If it's not on the scroll, report -1. An O(log n) solution is required.

## Examples

### 1

#### Input

7 0 
[4, 5, 6, 7, 0, 1, 2]


#### Output

4

#### Explanation

The key numbered 0 is at position 4 on the spun key ring.

### 2

#### Input

7 3 
[4, 5, 6, 7, 0, 1, 2]

#### Output

-1

#### Explanation

The key numbered 3 is not on this key ring.

## Input Format

- The first line contains an integers n and target , the number of keys on the ring and the number of the key to find.
- The second line contains n space-separated integers representing the key numbers after the ring was spun. All numbers are unique.

## Output Format

- Return the index (0-based position) of the target key if it exists else -1 if the target key is not found.

## Constraints

- 1 ≤ n ≤ 10^5
- 1 ≤ key_number, target ≤ 10^9
- The array is a rotation of a sorted array.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

binary-search, array