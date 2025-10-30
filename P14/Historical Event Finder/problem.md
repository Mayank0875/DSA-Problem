## Title

Historical Event Finder

## Slug

historical-event-finder

## Difficulty

Easy

## Description

You are given a timeline of N historical events, sorted by the year they occurred. You are researching events that happened in a specific `target` year. To find the end of this period, you must find the index of the first event in the timeline that occurred in a year *strictly greater* than the `target` year. This marks the beginning of the next era.

You must write an algorithm with O(log n) runtime complexity.

## Examples

### 1

#### Input

6 8
[2, 5, 8, 8, 8, 12]


#### Output

5

#### Explanation

The events from year 8 are at indices 2, 3, and 4. The first event from a year strictly greater than 8 is from year 12, located at index 5.

### 2

#### Input

6 6
[2, 5, 7, 8, 11, 12]

#### Output

2

#### Explanation

There is no event from year 6. The first event from a year strictly greater than 6 is from year 7, which is at index 2.

## Input Format

- The first line contains an integers n and target , the number of grimoires and the ID of the grimoire to find. 
- The second line contains n space-separated integers representing the sorted grimoire IDs.


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