## Title
Airline Flight Path

## Slug
airline-flight-path

## Difficulty
Medium

## Description
A pilot groups waypoints into legs. Each waypoint has an altitude.

The Pilot is working with a sequence of $n$ waypoints, where the $i$-th waypoint has a value of $a_i$.

The Pilot needs to create a **flight plan**. A flight plan involves dividing the sequence of $n$ waypoints into one or more contiguous legs such that every waypoint belongs to exactly one leg.

For a specific flight plan, the **fuel burn** is calculated as follows:
1. Calculate the sum of values for each leg in the partition.
2. The fuel burn is the bitwise XOR sum of these leg sums.

Your task is to calculate the bitwise XOR sum of the fuel burn values of **all possible flight plans** of the sequence.

## Examples

### 1

#### Input
1
1

#### Output
1

#### Explanation
Total XOR sum: 1.

### 2

#### Input
2
1 2

#### Output
0

#### Explanation
Partition {1}, {2}: Group sums are 1, 2. XOR sum = 1 ^ 2 = 3.
Partition {1, 2}: Group sum is 3. XOR sum = 3.
Total Result = 3 ^ 3 = 0.

## Input Format
- The first line contains a single integer $n$ — the length of the sequence.
- The second line contains $n$ space-separated integers $a_1, a_2, \dots, a_n$.

## Output Format
- Return a single integer representing the total XOR sum of fuel burns of all possible partitions.

## Constraints
- 1 ≤ n ≤ 10^6
- 1 ≤ a_i ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths, dynamic-programming, array
