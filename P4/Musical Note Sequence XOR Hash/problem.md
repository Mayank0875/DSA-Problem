## Title

Musical Note Sequence XOR Hash

## Slug

music-note-xor-hash

## Difficulty

Easy

## Description

A musicologist represents a melody as a sequence of numerical note values A₁, A₂, ..., Aₙ. To find recurring harmonic patterns, they analyze segments (windows) of size K. For each segment, a hash value is calculated by XORing the note values within the window. To get an overall hash representing the melody's structure, all segment hashes are XORed together. Compute this final melodic hash value.

## Examples

### 1

#### Input

5 3
[1, 2, 3, 4, 5]

#### Output

7

#### Explanation

Note sequence windows of size 3:
    •   [1, 2, 3] → Segment Hash (XOR) = 0
    •   [2, 3, 4] → Segment Hash (XOR) = 5
    •   [3, 4, 5] → Segment Hash (XOR) = 2

Final Melodic Hash = 0 ^ 5 ^ 2 = 7

### 2

#### Input

4 2
[5, 1, 3, 2]

#### Output

7

#### Explanation

Windows:
    •   [5, 1] → XOR = 4
    •   [1, 3] → XOR = 2
    •   [3, 2] → XOR = 1

Final Melodic Hash = 4 ^ 2 ^ 1 = 7

## Input Format

- The first line contains two integers N (number of notes) and K (window size).
- The second line contains N space-separated integers — the numerical note values.

## Output Format

- Return a single integer — the final melodic hash value.

## Constraints

- 1 ≤ N ≤ 10^5
- 1 ≤ K ≤ N
- 0 ≤ arr[i] ≤ 1e9

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

arrays, sliding window, music, bit manipulation