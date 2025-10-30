## Title

Robot Path Optimization

## Slug

robot-path-optimization

## Difficulty

Medium

## Description

A robot is given a sequence of N commands, 'Turn Left' (0) or 'Turn Right' (1). For the robot to end up facing its original direction after the sequence, the total number of Left and Right turns must be equal. You can optimize the robot's path by deleting exactly one contiguous sub-sequence of commands. Find the length of the shortest sub-sequence you can delete to balance the turns. If the path is already balanced, return 0.

## Examples

### 1

#### Input

6
[1, 0, 0, 0, 1, 0]

#### Output

2

#### Explanation

The path has four 'Left' (0) and two 'Right' (1) turns. To balance, we must remove two more 0s than 1s.
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