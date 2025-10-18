## Title

Gemstone Necklace Pivot

## Slug

gemstone-necklace-minimum

## Difficulty

Medium

## Description

A beautiful necklace is made of unique, numbered gemstones arranged in a circle. Originally, the gem numbers increased clockwise. However, the necklace clasp was moved, effectively rotating the sequence. 
For example, a sequence [10, 20, 30, 40, 50] might become [30, 40, 50, 10, 20]. 
To understand the necklace's original arrangement, a jeweler needs to find the gemstone with the smallest number. Given the sequence of gem numbers as they appear on the rotated necklace, find this minimum value efficiently.

You must write an algorithm with O(log n) runtime complexity

## Examples

### 1

#### Input

7 
[4, 5, 6, 7, 0, 1, 2]


#### Output

0

#### Explanation

The smallest gem number in this rotated sequence is 0.

### 2

#### Input

6 3 
[4, 5, 6, 7, 1, 2]

#### Output

1

#### Explanation

The smallest gem number in this rotated sequence is 1.

## Input Format

- The first line contains an integers n and target, the number of gemstones.
- The second line contains n space-separated integers representing the gem numbers after rotation. All numbers are unique.

## Output Format

- Return a single integer representing the minimum gem number found on the necklace.

## Constraints

- 1 ≤ n ≤ 10^5
- 1 ≤ gem_number ≤ 10^9
- The array is guaranteed to be a rotation of a sorted array.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

binary-search, array, rotated-array
