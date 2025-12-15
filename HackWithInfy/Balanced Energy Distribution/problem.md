## Title

Balanced Energy Distribution

## Slug

balanced-energy-distribution

## Difficulty

Hard

## Description

You are the chief engineer of a futuristic power plant. The plant generates a sequence of $n$ energy pulses, where the $i$-th pulse has an energy magnitude of $x_i$.

To safely store this energy, you must partition the continuous sequence of pulses into exactly $k$ non-empty contiguous segments. Each segment is assigned to a specific capacitor bank. The "stress" placed on a capacitor bank is calculated as the square of the sum of the energy pulses in that segment.

Your goal is to minimize the wear and tear on the system by finding a partition that minimizes the total stress (the sum of the stress values of all $k$ segments).

## Examples

### 1

#### Input

8 3
2 3 1 2 2 3 4 1

#### Output

110

#### Explanation

We partition the pulses into 3 segments: $[2, 3, 1]$, $[2, 2, 3]$, and $[4, 1]$.The sums are $6, 7, 5$.The total stress is $6^2 + 7^2 + 5^2 = 36 + 49 + 25 = 110$.
    
### 2

#### Input

5 1
1 2 3 4 5

#### Output

225

#### Explanation

Only 1 segment is allowed, containing all pulses. Sum = 15. Stress = $15^2 = 225$.

## Input Format  

- The first line contains two integers $n$ and $k$: the number of energy pulses and the required number of segments.
- The second line contains $n$ integers x_1, x_2, x_3 .. x_n: the magnitudes of the energy pulses.

## Output Format  

- Return one integer: the minimum total stress.
  

## Constraints  

- 1 ≤ k ≤ n ≤ 3000
- 1 ≤ x_i ≤ 1e5

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

dynamic-programming, array, hackwithinfy

## Companies
infosys