## Title

Circular Assembly Line

## Slug

circular-assembly-line

## Difficulty

Medium

## Description

A circular assembly line has stations numbered 1 to n. The parts on the line are sorted by their unique ID. The belt was stopped, and the list of parts now starts from an arbitrary station, effectively "rotating" the sorted list. For example, a sorted list [10, 20, 30, 40] might appear as [30, 40, 10, 20]. Given this rotated list and a target part ID, find its index on the line. An O(log n) solution is needed. Return -1 if the part is not found.

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