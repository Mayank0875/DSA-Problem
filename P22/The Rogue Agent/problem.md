## Title

The Rogue Agent

## Slug

the-rogue-agent

## Difficulty

Medium

## Description

In a spy agency, all field agents are assigned a partner. On the active agent list, sorted by codenumber, each agent's codenumber should appear twice in a row (for the agent and their partner). However, one agent is a "lone wolf" and has no partner; their codenumber appears only once. Find the codenumber of the lone wolf agent.

You must write an algorithm with O(log n) runtime complexity.

## Examples

### 1

#### Input

9 
[1, 1, 2, 3, 3, 4, 4, 8, 8]


#### Output

2

#### Explanation

In the sequence [1, 1, 2, 3, 3, 4, 4, 8, 8], the number 2 appears only once.

### 2

#### Input

7 
[3, 3, 7, 7, 10, 11, 11]

#### Output

10

#### Explanation

In the sequence [3, 3, 7, 7, 10, 11, 11], the number 10 appears only once.

## Input Format

- The first line contains an odd integer n, the total number of agent entries.
- The second line contains n space-separated integers representing the sorted agent codenumbers.

## Output Format

- Return a single integer: the codenumber of the agent that appears only once.

## Constraints

- 1 ≤ n ≤ 10^5
- 1 ≤ stone_value ≤ 10^9
- The array is sorted.
- Every element appears twice except for one.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

binary-search, array