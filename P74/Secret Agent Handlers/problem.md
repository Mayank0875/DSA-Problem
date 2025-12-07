## Title
Secret Agent Handlers

## Slug
secret-agent-handlers

## Difficulty
Medium

## Description
A spy network operates as a cell tree. To increase security, agents are pairing up with their direct contacts for a mission. Each agent can only be part of one pair.

The structure is a tree with n agents and n-1 contacts.
A mission pair is formed between two agents connected by a contact.
However, each agent can be part of at most one mission pair.

Your task is to calculate the maximum number of mission pairs that can be formed.

## Examples

### 1

#### Input
5
1 2
1 3
3 4
3 5

#### Output
2

#### Explanation
One optimal set of mission pairs is (1, 2) and (3, 4). Node 5 remains unpaired. This gives a total of 2 mission pairs.

### 2

#### Input
4
1 2
2 3
3 4

#### Output
2

#### Explanation
We can form mission pairs (1, 2) and (3, 4), giving a total of 2.

## Input Format
- The first line contains an integer n, the number of agents.
- The next n-1 lines each contain two integers u and v, representing a contact between agent u and agent v.

## Output Format
- Return a single integer representing the maximum number of mission pairs.

## Constraints
- 1 ≤ n ≤ 2e5
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, graph
