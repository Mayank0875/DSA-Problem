## Title

Guest Plus-Ones

## Slug

guest-plus-ones

## Difficulty

Easy

## Description

You are checking the RSVP list for a party. Each RSVP is an integer ID. An ID that appears exactly twice represents a guest who is bringing a 'plus-one'. Given the full list of RSVP IDs, find all IDs that are bringing a plus-one. Return them in increasing order. If no one is bringing just one guest, return an empty list.

## Examples

### 1
#### Input
8
1 2 2 3 3 3 4 4

#### Output
2 4

#### Explanation
2 appears twice, 4 appears twice. 3 appears thrice (maybe a family), 1 appears once (solo).

### 2
#### Input
5
5 5 5 6 7

#### Output


#### Explanation
No number appears exactly twice.

## Input Format
- First line: integer n — number of elements.
- Second line: n space-separated integers.

## Output Format
- Return all integers that appear exactly twice in increasing order, as a list/array. If none, return an empty list/array.

## Constraints
- 1 ≤ n ≤ 10^5
- Values fit in 32-bit signed integer

## Time Limit
1 second

## Memory Limit
256 MB

## Tags 
map, sorting