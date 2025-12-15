## Title
Spy Mission Protocol

## Slug
spy-mission-protocol

## Difficulty
Medium

## Description
Intelligence HQ pairs `n` agents with `m` missions.

However, not every agent is compatible with every mission due to security clearance.
You are given a list of `k` compatible pairs, where a specific agent can work with a specific mission.

Your task is to determine the maximum number of operations that can be formed simultaneously. Each agent and each mission can be assigned to at most one operation.

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
There are 3 agents and 2 missions.
Possible valid matching could be:
- agent 1 with mission 2
- agent 2 with mission 1
Total = 2.

### 2

#### Input
2 2 1
1 1

#### Output
1

#### Explanation
Only agent 1 and mission 1 are compatible. The maximum number of operational operations is 1.

## Input Format
- The first line contains three integers `n`, `m`, and `k`: the number of agents, missions, and compatible pairs.
- The agents are numbered `1` to `n` and the missions are numbered `1` to `m`.
- The next `k` lines describe the compatible pairs. Each line contains two integers `a` and `b`, indicating that agent `a` and mission `b` are compatible.

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
