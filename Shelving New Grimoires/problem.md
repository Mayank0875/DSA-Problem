## Title

Shelving New Grimoires

## Slug

shelving-new-grimoires

## Difficulty

Easy

## Description

The librarian has received a new grimoire and must place it on the correct shelf to maintain the sorted order of identification numbers. 
To do this, they need to find the position of the first grimoire whose ID is greater than or equal to the new grimoire's ID. 
If all existing grimoires have smaller IDs, the new one should be placed at the very end. Your task is to write an efficient function that takes the sorted list of grimoire IDs and the new ID, and returns the correct index for insertion.


You must write an algorithm with O(log n) runtime complexity

## Examples

### 1

#### Input

6 8
[2, 5, 7, 8, 11, 12]


#### Output

3

#### Explanation

The first grimoire with an ID greater than or equal to 8 is at index 3.

### 2

#### Input

6 6
[2, 5, 7, 8, 11, 12]

#### Output

2

#### Explanation

There is no grimoire with ID 6. The first grimoire with an ID greater than 6 is 7, which is at index 2.

## Input Format

- The first line contains an integers n and target , the number of grimoires and the ID of the grimoire to find. 
- The second line contains n space-separated integers representing the sorted grimoire IDs.
- You will be given the array as an input to your function

## Output Format

- Return a single integer representing the index of the first element that is greater than or equal to the target.


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
