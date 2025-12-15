## Title
Money Laundering

## Slug
money-laundering

## Difficulty
Medium

## Description
Dirty money is moving from a Shell Company (node 1) to a Clean Account (node n).

The banking network consists of $n$ accounts connected by $m$ two-way transactions.
The funds is attempting to travel from the Shell Company (node 1) to the Clean Account (node $n$).

To prevent this, you can freeze specific transactions. Freezing a transaction path stops the flow.

Your task is to calculate the **minimum number of transactions** that must be frozen to completely sever all routes between the Shell Company and the Clean Account.

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
We can freeze edges (1,3) and (2,3) to isolate node 3.

## Input Format
- The first line contains two integers $n$ and $m$: the number of accounts and transactions.
- The next $m$ lines describe the transactions. Each line contains two integers $a$ and $b$, indicating a transaction path between account $a$ and account $b$.

## Output Format
- Return one integer: the minimum number of transactions that need to be frozen.

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
