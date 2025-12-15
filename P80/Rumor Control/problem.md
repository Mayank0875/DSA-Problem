## Title
Rumor Control

## Slug
rumor-control

## Difficulty
Medium

## Description
A malicious rumor started with Person 1 and is spreading to the CEO (node n).

The social network consists of $n$ people connected by $m$ two-way friendships.
The rumor is attempting to travel from Person 1 (node 1) to the CEO (node $n$).

To prevent this, you can monitor specific friendships. Monitoring a friendship prevents gossip exchange.

Your task is to calculate the **minimum number of friendships** that must be monitored to completely sever all routes between Person 1 and the CEO.

## Examples

### 1

#### Input
4 5
1 2
1 3
2 3
3 4
1 4

#### Output
2

#### Explanation
The minimum is 2.

### 2

#### Input
3 3
1 2
2 3
1 3

#### Output
2

#### Explanation
We can monitor edges (1,3) and (2,3) to isolate node 3.

## Input Format
- The first line contains two integers $n$ and $m$: the number of people and friendships.
- The next $m$ lines describe the friendships. Each line contains two integers $a$ and $b$, indicating a friendship between person $a$ and person $b$.

## Output Format
- Return one integer: the minimum number of friendships that need to be monitored.

## Constraints
- 1 ≤ n ≤ 500
- 1 ≤ m ≤ 1000
- 1 ≤ a, b ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph
