## Title
Spy Message Drop

## Slug
spy-message-drop

## Difficulty
Medium

## Description
A spy network passes secret messages. Hand-off locations are compromised after one use.

The network consists of $n$ safehouses and $m$ one-way routes. Each route connects a specific source safehouse to a destination safehouse.

The process happens over several messages. In each message, you must send a courier from safehouse 1 (the source) to safehouse $n$ (the destination). The catch is that each route becomes watched by counter-intel after one use. This means each route can be used at most once across all messages combined.

Your goal is to determine the maximum number of messages you can successfully complete the journey from safehouse 1 to safehouse $n$.

## Examples

### 1

#### Input
6 7
1 2
1 3
2 6
3 4
3 5
4 6
5 6

#### Output
2

#### Explanation
You can complete 2 messages.
Path 1: 1 -> 2 -> 6
Path 2: 1 -> 3 -> 4 -> 6 (or 1 -> 3 -> 5 -> 6)

### 2

#### Input
2 1
1 2

#### Output
1

#### Explanation
You can complete 1 message.

## Input Format
- The first line contains two integers $n$ and $m$: the number of safehouses and the number of routes.
- The next $m$ lines describe the routes. Each line contains two integers $a$ and $b$, indicating a directed route from safehouse $a$ to safehouse $b$.

## Output Format
- Return one integer: the maximum number of messages possible.

## Constraints
- 1 ≤ n ≤ 500
- 1 ≤ m ≤ 1000
- 1 ≤ a, b ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph, breadth-first-search
