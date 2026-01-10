## Title
Conveyor Belt Check

## Slug
conveyor-belt-check

## Difficulty
Medium

## Description
Sensors on a belt turn green. The belt is 'monitored' if sensors 1 to k are green.

There is a sequence of $n$ sensors indexed from $1$ to $n$. Initially, all sensors are **red**.

You activate the sensors one by one in a specific order given by an array `sequence`. In the $i$-th step (1-indexed), you activate the sensor at the position `sequence[i-1]`.

A state is called **monitored** if, after performing $k$ steps, exactly the first $k$ sensors (indices $1$ to $k$) are green and all other sensors are red.

Your task is to calculate how many times the system becomes **monitored** during the entire process.

## Examples

### 1

#### Input
5
3 2 4 1 5

#### Output
2

#### Explanation
- Step 1 (index 3): "RRGRR" (Not monitored)
- Step 2 (index 2): "RGGRR" (Not monitored)
- Step 3 (index 4): "RGGGR" (Not monitored)
- Step 4 (index 1): "GGGGR" (monitored: first 4 are green)
- Step 5 (index 5): "GGGGG" (monitored: first 5 are green)
Total monitored states: 2.

### 2

#### Input
4
4 1 2 3

#### Output
1

#### Explanation
- Step 1 (index 4): "RRRG" (Not monitored)
- Step 2 (index 1): "GRRG" (Not monitored)
- Step 3 (index 2): "GGRG" (Not monitored)
- Step 4 (index 3): "GGGG" (monitored)
Total monitored states: 1.

## Input Format
- The first line contains an integer $n$.
- The second line contains $n$ space-separated integers representing the array `sequence`.

## Output Format
- Return a single integer representing the number of times the state was monitored.

## Constraints
- 1 ≤ n ≤ 10^4
- `sequence` is a permutation of numbers from $1$ to $n$.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, greedy

## Company
google
