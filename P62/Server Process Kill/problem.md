## Title
Server Process Kill

## Slug
server-process-kill

## Difficulty
Medium

## Description
A system admin must terminate k background processes to free up CPU. Processes are grouped by application ID. It is cleaner to stop all processes of a specific app. Determine the minimum number of unique application IDs running after the purge.

## Examples

### 1

#### Input
3 1
5 5 4

#### Output
1

#### Explanation
Remove the single item with ID 4. The remaining items are [5, 5]. The only unique ID left is 5. The count of unique types is 1.

### 2

#### Input
7 3
4 3 1 1 3 3 2

#### Output
2

#### Explanation
The item frequencies are: ID 3 (3 times), ID 1 (2 times), ID 4 (1 time), ID 2 (1 time).
To minimize unique types, remove the least frequent first.
Remove ID 4 (1 count) -> k becomes 2.
Remove ID 2 (1 count) -> k becomes 1.
Remove one instance of ID 1 -> k becomes 0.
Remaining types: ID 3 and ID 1. Total unique types left = 2.

## Input Format
- The first line contains integers n and k, the number of items and the number of items to remove.
- The second line contains n space-separated integers representing the item IDs.

## Output Format
- Return a single integer representing the least number of unique item types remaining.

## Constraints
- 1 ≤ n ≤ 10^5
- 1 ≤ k ≤ n
- 0 ≤ items[i] ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, hash-table, greedy, sorting
