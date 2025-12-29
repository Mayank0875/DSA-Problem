## Title

The Architect's Resonance

## Slug

the-architects-resonance

## Difficulty

Medium

## Description

Arin is a visionary architect designing a modular skyscraper. The building consists of $n$ vertical sections, where the `i`-th section has a structural weight of `a_i`.

Arin needs to finalize the blueprint by creating a **partition** of the building. A partition involves dividing the sequence of `n` sections into one or more contiguous groups (subarrays) such that every section belongs to exactly one group.

For a specific blueprint (partition), the `resonance` is calculated as follows:
1. Calculate the sum of weights for each group in the partition.
2. The resonance is the bitwise XOR sum of these group weights.

Arin wants to analyze the structural integrity of all possibilities. Your task is to calculate the bitwise XOR sum of the resonance values of `all possible partitions` of the array.

## Examples

### 1

#### Input

1
1

#### Output

1

#### Explanation

Total XOR sum: 1
    
### 2

#### Input

2
1 2

#### Output

0

#### Explanation

Total XOR sum: 0
  

## Input Format  

- The first line contains a single integer $n$ — the length of the array.
- The second line contains $n$ space-separated integers a_1, a_2, ...., a_n.

## Output Format  

- Return single integer representing the total XOR sum of resonances of all possible partitions.
  

## Constraints  

- 1 ≤ n ≤ 1e6
- 1 ≤ a_i ≤ 1e9

## Time Limit

1 second

## Memory Limit

256 MB

## Tags

binary-search, maths, array, hackwithinfy

## Companies
infosys
