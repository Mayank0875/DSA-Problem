## Title

The Lost Grimoire

## Slug

lost-grimoire

## Difficulty

Easy

## Description

An ancient library contains countless magical grimoires, all neatly arranged on a single, vast shelf and sorted by a unique identification number. 
A librarian needs to quickly check if a specific grimoire is on this shelf without searching one by one. Your task is to create a function that takes the sorted list of grimoire IDs and a target ID as input. 
The function should efficiently determine whether the grimoire is present and return 1 if present otherwise 0 . The grimoire IDs are sorted in non-decreasing order.

You must write an algorithm with O(log n) runtime complexity

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

- Return True if the grimoire is found, and False otherwise.

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
