## Title
Hospital Ward Rounds

## Slug
hospital-ward-rounds

## Difficulty
Hard

## Description
A hospital wing has `n` patients. `k` doctors split the rounds. Patients are visited in room order. The 'mental load' on a doctor is the square of the total acuity scores of the patients they see.

You must partition the sequence of patients into exactly `k` non-empty contiguous rounds.
Each round corresponds to a doctor.
The "mental load" for a doctor is calculated as the **square of the sum** of the acuity scores of the patients in that round.

Your goal is to minimize the total mental load (the sum of the mental load values of all `k` rounds).

## Examples

### 1

#### Input
8 3
2 3 1 2 2 3 4 1

#### Output
110

#### Explanation
We partition the patients into 3 rounds: `[2, 3, 1]`, `[2, 2, 3]`, and `[4, 1]`.
The sums are 6, 7, 5.
The total mental load is $6^2 + 7^2 + 5^2 = 36 + 49 + 25 = 110$.

### 2

#### Input
5 1
1 2 3 4 5

#### Output
225

#### Explanation
Only 1 round is allowed, containing all patients. Sum = 15. mental load = $15^2 = 225$.

## Input Format
- The first line contains two integers `n` and `k`: the number of patients and the required number of rounds.
- The second line contains `n` integers representing the acuity scores of each patient.

## Output Format
- Return one integer: the minimum total mental load.

## Constraints
- 1 ≤ k ≤ n ≤ 3000
- 1 ≤ value ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, array
