## Title
Elevator Passenger Groups

## Slug
elevator-passenger-groups

## Difficulty
Hard

## Description
A line of `n` people waits for elevators. There are `k` elevators available. People board in order. The 'cable strain' on an elevator is the square of the total weight of its passengers.

You must partition the sequence of people into exactly `k` non-empty contiguous loads.
Each load corresponds to a elevator.
The "cable strain" for a elevator is calculated as the **square of the sum** of the weights of the people in that load.

Your goal is to minimize the total cable strain (the sum of the cable strain values of all `k` loads).

## Examples

### 1

#### Input
8 3
2 3 1 2 2 3 4 1

#### Output
110

#### Explanation
We partition the people into 3 loads: `[2, 3, 1]`, `[2, 2, 3]`, and `[4, 1]`.
The sums are 6, 7, 5.
The total cable strain is $6^2 + 7^2 + 5^2 = 36 + 49 + 25 = 110$.

### 2

#### Input
5 1
1 2 3 4 5

#### Output
225

#### Explanation
Only 1 load is allowed, containing all people. Sum = 15. cable strain = $15^2 = 225$.

## Input Format
- The first line contains two integers `n` and `k`: the number of people and the required number of loads.
- The second line contains `n` integers representing the weights of each person.

## Output Format
- Return one integer: the minimum total cable strain.

## Constraints
- 1 ≤ k ≤ n ≤ 3000
- 1 ≤ value ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, array
