## Title
Signal Interference Cancellation

## Slug
signal-interference-cancellation

## Difficulty
Easy

## Description
A telecommunications engineer is trying to filter out background noise from a radio transmission. The background noise has a specific power level. The engineer has identified several interference sources, each producing a signal with a specific amplitude. In signal processing, the power of a signal is often represented as the square of its amplitude. To deploy a counter-signal, the engineer needs to identify if the noise is being caused by the combination of exactly three interference sources summing up to the measured noise power level.

Your task is to determine whether it is possible to choose three distinct signal sources (at indices i < j < k) such that:

    amplitude_i^2 + amplitude_j^2 + amplitude_k^2 = noise_power

If it is possible, print YES; otherwise, print NO.

## Examples

### 1
#### Input
5
1 2 2 3 4
9

#### Output
YES

#### Explanation
1^2 + 2^2 + 2^2 = 1 + 4 + 4 = 9.

### 2
#### Input
4
3 3 3 3
20

#### Output
NO

#### Explanation
Every square is 9; any sum of three squares is 27 which is not 20.

## Input Format
- First line: integer n — the number of signal sources.
- Second line: n space-separated integers a1 a2 ... an — the amplitudes (can be negative, zero, or positive).
- Third line: integer target — the target sum.

## Output Format
- Return true (YES) if there exist indices i < j < k with a[i]^2 + a[j]^2 + a[k]^2 = target, otherwise return false (NO).

## Constraints
- 3 ≤ n ≤ 2000
- -10^6 ≤ ai ≤ 10^6
- 0 ≤ target ≤ 3×10^12

## Time Limit
1 second

## Memory Limit
256 MB

## Tags 
two-pointers, sorting, array, maths
