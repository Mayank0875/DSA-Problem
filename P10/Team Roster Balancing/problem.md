## Title

Team Roster Balancing

## Slug

team-roster-balancing

## Difficulty

Medium

## Description

A coach is building a sports team from a linear tryout list of N players. Each player is classified as either 'Offense' (1) or 'Defense' (0). For a perfectly balanced team, the coach needs an equal number of offensive and defensive players. The coach can select their team by removing exactly one contiguous group of players from the tryout list. Your task is to find the length of the shortest contiguous group of players to remove to achieve this balance. If the list is already balanced, the length is 0.

## Examples

### 1

#### Input

6
[1, 0, 0, 0, 1, 0]

#### Output

2

#### Explanation

The initial list has two 'Offense' (1) and four 'Defense' (0). To balance, we must remove a segment with two more 0s than 1s.
The shortest segment that achieves this is [0, 0] at indices 2 and 3. 
The length of the removed segment is 2.


### 2

#### Input

6
[1, 1, 0, 0, 1, 0,]

#### Output

0

#### Explanation

The stream contains three 0s and three 1s. It is already balanced, so no segment needs to be removed. 
The length of the removed segment is 0.


## Input Format

- The first line contains a single integer N, the number of elements in the data stream.
- The second line contains N space-separated integers, where each integer is either 0 or 1.

## Output Format

- Return a single integer representing the length of the shortest contiguous segment that needs to be removed to balance the stream.

## Constraints

- 1 ≤ N ≤ 10^5
- 0 ≤ arr[i] ≤ 1

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

arrays, sliding window, prefix sum, hashmap