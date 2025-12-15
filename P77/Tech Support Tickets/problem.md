## Title
Tech Support Tickets

## Slug
tech-support-tickets

## Difficulty
Medium

## Description
A helpdesk routes `n` tickets to `m` support agents.

However, not every ticket is compatible with every agent based on problem category.
You are given a list of `k` compatible pairs, where a specific ticket can work with a specific agent.

Your task is to determine the maximum number of resolutions that can be formed simultaneously. Each ticket and each agent can be assigned to at most one resolution.

## Examples

### 1

#### Input
3 2 4
1 1
1 2
2 1
3 1

#### Output
2

#### Explanation
There are 3 tickets and 2 agents.
Possible valid matching could be:
- ticket 1 with agent 2
- ticket 2 with agent 1
Total = 2.

### 2

#### Input
2 2 1
1 1

#### Output
1

#### Explanation
Only ticket 1 and agent 1 are compatible. The maximum number of operational resolutions is 1.

## Input Format
- The first line contains three integers `n`, `m`, and `k`: the number of tickets, agents, and compatible pairs.
- The tickets are numbered `1` to `n` and the agents are numbered `1` to `m`.
- The next `k` lines describe the compatible pairs. Each line contains two integers `a` and `b`, indicating that ticket `a` and agent `b` are compatible.

## Output Format
- Return one integer: the maximum number of pairs that can be formed.

## Constraints
- 1 ≤ n, m ≤ 500
- 1 ≤ k ≤ 1000
- 1 ≤ a ≤ n
- 1 ≤ b ≤ m

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph
