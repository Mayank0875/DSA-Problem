## Title
Information Leak

## Slug
information-leak

## Difficulty
Medium

## Description
A whistleblower at the Agency (node 1) sends files to the Press (node n).

The comm network consists of $n$ relays connected by $m$ two-way channels.
The files is attempting to travel from the Agency (node 1) to the Press (node $n$).

To prevent this, you can encrypt specific channels. Disabling a channel stops the leak.

Your task is to calculate the **minimum number of channels** that must be disabled to completely sever all routes between the Agency and the Press.

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
We can encrypt edges (1,3) and (2,3) to isolate node 3.

## Input Format
- The first line contains two integers $n$ and $m$: the number of relays and channels.
- The next $m$ lines describe the channels. Each line contains two integers $a$ and $b$, indicating a channel between relay $a$ and relay $b$.

## Output Format
- Return one integer: the minimum number of channels that need to be disabled.

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
