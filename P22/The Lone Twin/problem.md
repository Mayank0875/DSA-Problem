## Title

The Lone Twin

## Slug

the-lone-twin

## Difficulty

Medium

## Description

You are a photographer at a convention for identical twins. All attendees are lined up, sorted by their ID number. Every person is standing next to their identical twin, forming pairs. However, one person attended the convention without their twin and is the only person without a pair. Given the sorted list of IDs, find the ID of the person who is alone.

You must write an algorithm with O(log n) runtime complexity.

## Examples

### 1

#### Input

9 
[1, 1, 2, 3, 3, 4, 4, 8, 8]


#### Output

2

#### Explanation

In the sequence [1, 1, 2, 3, 3, 4, 4, 8, 8], the number 2 appears only once.

### 2

#### Input

7 
[3, 3, 7, 7, 10, 11, 11]

#### Output

10

#### Explanation

In the sequence [3, 3, 7, 7, 10, 11, 11], the number 10 appears only once.

## Input Format

- The first line contains an odd integer n, the total number of attendees.
- The second line contains n space-separated integers representing the sorted attendee IDs.

## Output Format

- Return a single integer: the ID of the attendee who appears only once.

## Constraints

- 1 ≤ n ≤ 10^5
- 1 ≤ stone_value ≤ 10^9
- The array is sorted.
- Every element appears twice except for one.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

binary-search, array