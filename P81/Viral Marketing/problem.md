## Title
Viral Marketing

## Slug
viral-marketing

## Difficulty
Medium

## Description
An ad is viewed by User 1 and shared until it reaches Influencer n.

The social media has `n` users and `m` directed shares. Shares may repeat between the same pair of users and self-loops are allowed. A campaign path of length `k` is a sequence of exactly `k` directed shares; users and shares may be visited multiple times.

Given `n`, `m`, `k` and a list of the `m` directed shares (each share given as two integers `u` `v` meaning a directed share from `u` to `v`), compute the number of distinct campaign paths that start at user 1 and end at user `n` with length exactly `k`. Output the answer modulo 1000000007.

## Examples

### 1

#### Input
3 4 8
1 2
2 3
3 1
3 2

#### Output
2

#### Explanation
We have 3 users. We want the number of directed campaign paths of length 8 from user 1 to user 3.
Valid length-8 campaign paths:
1 -> 2 -> 3 -> 1 -> 2 -> 3 -> 1 -> 2 -> 3
1 -> 2 -> 3 -> 2 -> 3 -> 1 -> 2 -> 3
There are 2 such campaign paths.

### 2

#### Input
3 4 2
1 2
2 3
3 1
3 2

#### Output
1

#### Explanation
Assuming the graph has shares 1->2 and 2->3, the only campaign path of length 2 from user 1 to user 3 is:
1 -> 2 -> 3

## Input Format
- The first line contains three integers n, m, and k: the number of users, shares, and the required campaign path length.
- The next m lines describe the shares. Each line contains two integers u and v, indicating a directed share from user u to user v.

## Output Format
- Return single integer: the number of campaign paths modulo 10^9+7.

## Constraints
- 1 ≤ n ≤ 100
- 1 ≤ m ≤ 10^5
- 1 ≤ k ≤ 10^18
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph, dynamic-programming
