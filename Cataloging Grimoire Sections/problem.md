## Title

Cataloging Grimoire Sections

## Slug

cataloging-grimoire-section

## Difficulty

Easy

## Description

The librarian needs to catalog sections of grimoires that share the same identification number. 
To find the end of the section for a given ID, they must locate the first grimoire on the shelf with an ID that is strictly greater than the target ID. This position marks the boundary where the next section begins. If no grimoire has a greater ID, the section extends to the end of the shelf.
Your task is to write a function that helps the librarian by quickly finding this boundary index.


You must write an algorithm with O(log n) runtime complexity

## Examples

### 1

#### Input

6 8
[2, 5, 8, 8, 8, 12]


#### Output

5

#### Explanation

The grimoires with ID 8 are at indices 2, 3, and 4. The first grimoire with an ID strictly greater than 8 is 12, located at index 5.

### 2

#### Input

6 6
[2, 5, 7, 8, 11, 12]

#### Output

2

#### Explanation

There is no grimoire with ID 6. The first grimoire with an ID strictly greater than 6 is 7, which is at index 2.
## Input Format

- The first line contains an integers n and target , the number of grimoires and the ID of the grimoire to find. 
- The second line contains n space-separated integers representing the sorted grimoire IDs.
- You will be given the array as an input to your function

## Output Format

- Return a single integer representing the index of the first element strictly greater than the target.

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
