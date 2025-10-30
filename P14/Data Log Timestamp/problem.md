## Title

Data Log Timestamp

## Slug

data-log-timestamp

## Difficulty

Easy

## Description

A server's log file contains N entries sorted by timestamp. You need to analyze all entries from a specific `target` timestamp. To do this, you must find the index of the first log entry with a timestamp *strictly greater* than the `target`. This marks the first entry that is not part of your analysis group.

You must write an algorithm with O(log n) runtime complexity.

## Examples

### 1

#### Input

6 8
[2, 5, 8, 8, 8, 12]


#### Output

5

#### Explanation

The logs with timestamp 8 are at indices 2, 3, and 4. The first log with a timestamp strictly greater than 8 is 12, located at index 5.

### 2

#### Input

6 6
[2, 5, 7, 8, 11, 12]

#### Output

2

#### Explanation

There is no log with timestamp 6. The first log with a timestamp strictly greater than 6 is 7, which is at index 2.

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