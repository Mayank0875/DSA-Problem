## Title

Librarian's Inventory Count

## Slug

librarians-inventory-count

## Difficulty

Medium

## Description

The Head Librarian of the Grand Archives is performing a complete inventory. For any given manuscript ID, they need to know exactly how many copies are on the shelf. 
The manuscripts are sorted by their ID, with all identical copies placed consecutively. 
Your job is to create a function that can quickly count the number of occurrences of any manuscript ID. The function will receive the sorted list of IDs and a target ID, and it should return the total count of that ID in the list.


You must write an algorithm with O(log n) runtime complexity

## Examples

### 1

#### Input

6 8
[2, 8, 8, 8, 11, 12]


#### Output

3

#### Explanation

The target ID 8 appears 3 times in the list.

### 2

#### Input

6 6
[2, 5, 7, 8, 11, 12]

#### Output

0

#### Explanation

The target ID 6 appears 0 times in the list.

## Input Format

- The first line contains an integers n and target , the number of manuscripts and the the ID to count.
- The second line contains n space-separated integers representing the sorted manuscript IDs.

## Output Format

- Return a single integer representing the total number of times the target appears.

## Constraints

- 1 ≤ n ≤ 10^5
- 1 ≤ manuscript_id, target ≤ 10^9
- The manuscript IDs are sorted in non-decreasing order.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

binary-search, array, counting
