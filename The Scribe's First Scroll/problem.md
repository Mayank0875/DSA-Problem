## Title

The Scribe's First Scroll

## Slug

scribes-first-scroll

## Difficulty

Easy

## Description

A historian is searching for the earliest known copy of a famous text in a vast, sorted archive. The archive contains many scrolls, some of which are identical copies, shelved consecutively according to their identification number. To begin their research, the historian needs to find the index of the very first scroll with a specific ID. 
Your task is to write a function that takes the sorted list of scroll IDs and a target ID, and returns the index of its first appearance. If the scroll is not in the archive, you should indicate this by returning -1.


You must write an algorithm with O(log n) runtime complexity

## Examples

### 1

#### Input

6 8
[2, 5, 7, 8, 11, 12]


#### Output

3

#### Explanation

The target ID 8 first appears at index 3.

### 2

#### Input

6 6
[2, 5, 7, 8, 11, 12]

#### Output

-1

#### Explanation

The target ID 6 is not found in the list.

## Input Format

- The first line contains an integers n and target , the number of scrolls and the ID of the scroll to find.
- The second line contains n space-separated integers representing the sorted grimoire IDs.

## Output Format

- Return a single integer: the index of the first occurrence of the target, or -1 if it is not found.

## Constraints

- 1 ≤ n ≤ 10^5
- 1 ≤ scroll_id, target ≤ 10^9
- The scroll IDs are sorted in non-decreasing order.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

binary-search, array, searching, first-occurrence
