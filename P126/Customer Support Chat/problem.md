## Title
Customer Support Chat

## Slug
customer-support-chat

## Difficulty
Easy

## Description
A support center tracks chat durations.

The chat system records the chat start and chat end of every agent in two integer arrays, `startTime` and `endTime`. The $i$-th agent starts a chat at `startTime[i]` and ends a chat at `endTime[i]`, inclusive.

The supervisor wants to know how many agents were busy during a specific high volume interval `[queryStart, queryEnd]`. A agent is considered busy if their conversation overlaps with the high volume interval at any point (even for a single moment).

Your task is to return the total number of agents who were busy during the given high volume interval.

## Examples

### 1

#### Input
3
1 2 3
3 2 7
2 4

#### Output
3

#### Explanation
The high volume interval is `[2, 4]`.
- Agent 1 `[1, 3]` overlaps with `[2, 4]` (times 2, 3).
- Agent 2 `[2, 2]` overlaps with `[2, 4]` (time 2).
- Agent 3 `[3, 7]` overlaps with `[2, 4]` (times 3, 4).
All 3 agents were busy.

### 2

#### Input
1
4
4
1 3

#### Output
0

#### Explanation
The agent was busy at time `[4, 4]`. The high volume interval is `[1, 3]`. There is no overlap.

## Input Format
- The first line contains an integer `n`, the number of agents.
- The second line contains `n` space-separated integers for `startTime`.
- The third line contains `n` space-separated integers for `endTime`.
- The fourth line contains two integers, `queryStart` and `queryEnd`.

## Output Format
- Return a single integer representing the number of agents busy during the high volume interval.

## Constraints
- 1 ≤ n ≤ 10^5
- 1 ≤ startTime[i] ≤ endTime[i] ≤ 10^9
- 1 ≤ queryStart ≤ queryEnd ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, interval, linear-scan

## Company
amazon
