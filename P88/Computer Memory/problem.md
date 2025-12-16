## Title
Computer Memory

## Slug
computer-memory

## Difficulty
Medium

## Description
Processes consume different amounts of RAM. To force a system swap, a group of active processes must use more than half the total RAM.

Your task is to count the number of **process groupss**. A process group is considered valid if it satisfies two specific criteria:
1.  **Swap Trigger:** The total RAM usage of the process group is strictly greater than half of the total RAM usage across all processes.
2.  **No Superfluous processes:** The process group is minimal. This means that removing **any one** process from the process group would cause the remaining total to drop to half or less of the total RAM usage (losing the Swap Trigger).

## Examples

### 1

#### Input
5
3 1 4 1 5

#### Output
4

#### Explanation
Total RAM usage is 14. Half is 7. We need a sum > 7.
The group {5, 4, 1} (Sum 10) is **not** valid because removing 1 leaves 9, which is still > 7.
Valid groups are those where every member is critical.

### 2

#### Input
4
1 2 3 4

#### Output
3

#### Explanation
Total RAM usage = 10. Half = 5.
Valid process groupss: {4, 2}, {4, 3}, {3, 2, 1}.

## Input Format
- The first line contains an integer n: the number of processes.
- The second line contains n integers: the RAM usage of each process.

## Output Format
- Return one integer: the total number of valid process groupss.

## Constraints
- 1 ≤ n ≤ 60
- 1 ≤ RAM usage ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths, dynamic-programming
