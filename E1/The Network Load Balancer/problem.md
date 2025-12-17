## Title
The Network Load Balancer

## Slug
network-load-balancer

## Difficulty
Easy

## Description
In a distributed computing system, a stream of data packets is waiting in a linear buffer. Each packet has a specific size in kilobytes. To optimize parallel processing, the system needs to spawn a worker process at a specific packet index. This packet will be the 'Processing Node'. The requirement is that the total data load (sum of sizes) of all packets preceding this node must equal the total data load of all packets succeeding it. Finding this node allows the system to split the remaining work into two equal threads.

You are given an array `nums` representing data packets in a queue. A Processing Node is an index where the sum of all packet sizes strictly to its left is equal to the sum of all packet sizes strictly to its right. If the pivot lies at an edge, the missing side is treated as having a sum of 0. Your task is to return the leftmost such Processing Node. If no such point exists, return -1.

## Examples

### 1

#### Input

nums = [1, 7, 3, 6, 5, 6]

#### Output

3

#### Explanation

For index 3 (value = 6):
Left side sum = 1 + 7 + 3 = 11
Right side sum = 5 + 6 = 11
Both sides are equal, so index 3 is a Processing Node.
It is also the leftmost such index.


### 2

#### Input

nums = [1, 2, 3]

#### Output

-1

#### Explanation

Index 0: left sum = 0, right sum = 2 + 3 = 5 (not equal)
Index 1: left sum = 1, right sum = 3 (not equal)
Index 2: left sum = 1 + 2 = 3, right sum = 0 (not equal)
No index has equal left and right sum, so answer is -1.


### 3

#### Input

nums = [2, 1, -1]

#### Output

0

#### Explanation

At index 0:
Left sum = 0
Right sum = 1 + (-1) = 0
Both sides are equal, so index 0 is a Processing Node.
Since it is the first index, it is the leftmost pivot.


## Input Format

- A single line containing an integer array `nums`.

## Output Format

- Return the index representing the leftmost pivot, or -1 if no such pivot exists.

## Constraints

- 1 ≤ nums.length ≤ 10⁴
- -1000 ≤ nums[i] ≤ 1000

## Time Limit

1 second

## Memory Limit

256 MB

## Tags

array, prefix-sum
