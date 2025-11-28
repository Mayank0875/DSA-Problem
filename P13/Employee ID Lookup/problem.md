## Title

Employee ID Lookup

## Slug

employee-id-lookup

## Difficulty

Easy

## Description

A company's HR department maintains a sorted list of all employee
identification numbers. For a payroll check, they need to verify if a
`target` ID is present in their system.
You must write an algorithm with O(log n) runtime complexity.

## Examples

### 1

#### Input

6 8
[2, 5, 7, 8, 11, 12]


#### Output

1

#### Explanation

The target ID 8 is found in the list of employee IDs.

### 2

#### Input

6 6
[2, 5, 7, 8, 11, 12]

#### Output

0

#### Explanation

The target ID 6 is not found in the list.

## Input Format

- The first line contains an integers n and target , the number of employees ID's and the ID to find. 
- The second line contains n space-separated integers representing the sorted employee IDs.

## Output Format

- Return 1 if the target is found, and 0 otherwise.

## Constraints

- 1 ≤ n ≤ 10^5
- 1 ≤ employee_id, target ≤ 10^9
- The employee IDs are sorted in non-decreasing order.

## Time Limit

1 second

## Memory Limit

256 MB

## Tags

binary-search, array
