## Title

Employee ID Lookup

## Slug

employee-id-lookup

## Difficulty

Easy

## Description

A company's HR department maintains a sorted list of all employee identification numbers. For a payroll check, they need to verify if a `target` ID is present in their system. Your task is to write this high-speed lookup function. You will be given the sorted list of IDs and the `target` ID to find. You must write an algorithm with O(log n) runtime complexity.

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

- The first line contains an integers n and target , the number of ID's and the ID to find. 
- The second line contains n space-separated integers representing the sorted IDs.

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

binary-search, array
