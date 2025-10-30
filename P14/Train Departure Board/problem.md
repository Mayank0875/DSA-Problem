## Title

Train Departure Board

## Slug

train-departure-board

## Difficulty

Easy

## Description

You are looking at a train departure board that lists N trains, sorted by their departure time. You want to see all trains departing at a specific `target` time. To see what's next, you must find the index of the first train on the board that departs at a time *strictly greater* than the `target` time.

You must write an algorithm with O(log n) runtime complexity.

## Examples

### 1

#### Input

6 8
[2, 5, 8, 8, 8, 12]


#### Output

5

#### Explanation

The trains departing at time 8 are at indices 2, 3, and 4. The first train departing at a time strictly greater than 8 is at time 12, located at index 5.

### 2

#### Input

6 6
[2, 5, 7, 8, 11, 12]

#### Output

2

#### Explanation

There is no train departing at time 6. The first train departing at a time strictly greater than 6 is at time 7, which is at index 2.

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