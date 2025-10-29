## Title

Allocating Bandwidth Channels

## Slug

allocating-bandwidth-channels

## Difficulty

Easy

## Description

An internet service provider needs to allocate users to communication channels. Each channel can support either one or two users. However, the total bandwidth requested by the user(s) on a single channel cannot exceed the channel's capacity `x`. You are given the bandwidth requirements for `n` users. Determine the minimum number of channels needed to serve all users without exceeding the bandwidth capacity on any channel.

## Examples

### 1

#### Input

4 10
[7, 2, 3, 9]

#### Output

3

#### Explanation

One efficient allocation:
    - Channel 1: User requiring 2 units and user requiring 7 units (Total 9 <= 10)
    - Channel 2: User requiring 3 units (Total 3 <= 10)
    - Channel 3: User requiring 9 units (Total 9 <= 10)
This requires 3 channels.

### 2

#### Input

5 5
[2, 2, 2, 3, 4]

#### Output

3

#### Explanation

One efficient allocation:
    - Channel 1: User requiring 2 units and user requiring 3 units (Total 5 <= 5)
    - Channel 2: Two users requiring 2 units (Total 4 <= 5)
    - Channel 3: User requiring 4 units (Total 4 <= 5)
This requires 3 channels.

## Input Format

- The first line contains two integers n and x: the number of users and the maximum bandwidth capacity per channel.
- The second line contains n integers p_1, p_2, ..., p_n: the bandwidth requirement of each user.

## Output Format

- Return a single integer: the minimum number of channels required.

## Constraints

- 1 ≤ n ≤ 1e5
- 1 ≤ x ≤ 1e9
- 1 ≤ p_i ≤ x

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

greedy, sorting, two pointers