## Title

Operation Blockade

## Slug

operation-blockade

## Difficulty

Medium

## Description

A notorious spy, Agent K, has just stolen sensitive data from the Central Bank (node 1) and is attempting to flee to the Extraction Point at the Harbor (node $n$). The city consists of $n$ intersections connected by $m$ two-way streets.

To prevent Agent K's escape, the police force plans to blockade specific streets. Blocking a street effectively cuts off travel in both directions between the two intersections it connects.

Your task is to calculate the **minimum number of streets** that must be blocked to completely sever all routes between the Bank and the Harbor.

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

We can block edges $(1,3)$ and $(2,3)$ to isolate node 3.
  

## Input Format  

- The first line contains two integers $n$ and $m$: the number of intersections and streets.
- The next $m$ lines describe the streets. Each line contains two integers $a$ and $b$, indicating a street between intersection $a$ and intersection $b$.

## Output Format  

- Return one integer: the minimum number of streets that need to be blocked.
  

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