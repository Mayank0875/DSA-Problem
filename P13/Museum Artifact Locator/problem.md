## Title

Museum Artifact Locator

## Slug

museum-artifact-locator

## Difficulty

Easy

## Description

A large museum archives its artifacts using a unique serial number. In the main database, these serial numbers are stored in a single, sorted list. A curator needs to verify if an artifact with a `target` serial number is part of the collection. Your job is to create a function that takes the sorted list of serial numbers and the target serial number, and efficiently confirms its presence. You must write an algorithm with O(log n) runtime complexity.

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

- The first line contains an integers n and target , the number of grimoires and the ID of the grimoire to find. 
- The second line contains n space-separated integers representing the sorted grimoire IDs.

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

binary-search, array, searching