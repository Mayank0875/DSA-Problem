## Title

Encrypted Valley Storage

## Slug

encrypted-valley

## Difficulty

Medium

## Description

In the hidden Encrypted Valley, the guardians must store n identical rectangular data crystals. Each crystal is w units wide and h units long. To protect the secrets, all crystals must be placed flat inside a single square vault. The crystals cannot be rotated. Your task is to help the guardians find the side length of the smallest possible square vault that can hold all n crystals without any overlap.

## Examples

### 1

#### Input

2 3 10

#### Output

9

#### Explanation

A square of side 9 fits ⌊9/2⌋ = 4 crystals across and ⌊9/3⌋ = 3 crystals down, giving 4 × 3 = 12 crystals — enough for 10.  
A square of side 8 fits ⌊8/2⌋ × ⌊8/3⌋ = 4 × 2 = 8 crystals — not enough.  
Hence, the minimum side length is 9.

### 2

#### Input

1 1 3

#### Output

2

#### Explanation

A square of side 2 fits ⌊2/1⌋ × ⌊2/1⌋ = 2 × 2 = 4 crystals.  
A square of side 1 fits only 1 × 1 = 1 crystal.  
Therefore, the minimum side length needed for 3 crystals is 2.
  
## Input Format  

- Three space-separated integers w, h, and n.

## Output Format  

- Return single integer representing the minimum side length of the square vault.
  

## Constraints  

- 1 ≤ w, h, n ≤ 1e6

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

binary-search, math, number-theory