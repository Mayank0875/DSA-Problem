## Title
Carrier Pigeon

## Slug
carrier-pigeon

## Difficulty
Medium

## Description
Pigeons fly between coops. Birds are retired after one long flight.

The courier net consists of $n$ coops and $m$ one-way flights. Each flight connects a specific source coop to a destination coop.

The process happens over several messages. In each message, you must send a pigeon from coop 1 (the source) to coop $n$ (the destination). The catch is that each flight tires the bird out completely. This means each flight can be used at most once across all messages combined.

Your goal is to determine the maximum number of messages you can successfully complete the journey from coop 1 to coop $n$.

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
- The first line contains two integers $n$ and $m$: the number of coops and the number of flights.
- The next $m$ lines describe the flights. Each line contains two integers $a$ and $b$, indicating a directed flight from coop $a$ to coop $b$.

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
