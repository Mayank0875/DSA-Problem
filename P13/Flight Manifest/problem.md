## Title

Flight Manifest

## Slug

flight-manifest

## Difficulty

Easy

## Description


An airline's flight manifest is a sorted list of all passenger
reservation numbers. A passenger arrives at the gate with their `target`
reservation number. You need to write the software that checks if this
`target` number is on the manifest. The check must be as fast as
possible. You must write an algorithm with O(log n) runtime complexity.

## Examples

### 1

#### Input

6 8
[2, 5, 7, 8, 11, 12]


#### Output

1

#### Explanation

The target reservation number 8 is found in the manifest.

### 2

#### Input

6 6
[2, 5, 7, 8, 11, 12]

#### Output

0

#### Explanation


The target reservation number 6 is not found in the manifest.

## Input Format


-   The first line contains two integers n and target, the number of
    reservation numbers and the reservation number to find.
-   The second line contains n space-separated integers representing the
    sorted reservation numbers

## Output Format

- Return 1 if the target is found, and 0 otherwise.

## Constraints

- 1 ≤ n ≤ 10^5
- 1 ≤ reservation_number, target ≤ 10^9
- The reservation number are sorted in non-decreasing order.

## Time Limit

1 second

## Memory Limit

256 MB

## Tags

binary-search, array, searching
