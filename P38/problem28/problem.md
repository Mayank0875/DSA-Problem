## Title

The Obsidian Key

## Slug

the-obsidian-key

## Difficulty

Easy

## Description

You are exploring an ancient dungeon where each chamber contains an obsidian key of a certain weight. For every chamber, you need to determine the weight of the key found in the nearest previous chamber that is strictly lighter than the key in the current chamber. If no such earlier chamber exists (either because it is the first chamber or all previous keys are heavier or equal), you should indicate this with -1. This information helps you understand the progression of key weights as you delve deeper. Compute this value for every chamber given the sequence of key weights.

## Examples

### 1

#### Input

8
[100, 80, 60, 70, 60, 75, 85, 110]

#### Output

[-1, -1, -1, 60, -1, 60, 75, 85]

#### Explanation

Chamber 0 (100): No previous chamber, output -1.  
Chamber 1 (80): Key 100 in chamber 0 is not lighter, output -1.  
Chamber 2 (60): Keys 100, 80 are not lighter, output -1.  
Chamber 3 (70): Key 60 in chamber 2 is lighter, output 60.  
Chamber 4 (60): Keys 100, 80, 60, 70. None are strictly lighter, output -1.  
Chamber 5 (75): Key 60 in chamber 4 is the nearest lighter, output 60.  
Chamber 6 (85): Key 75 in chamber 5 is the nearest lighter, output 75.  
Chamber 7 (110): Key 85 in chamber 6 is the nearest lighter, output 85.

### 2

#### Input

5
50 50 50 50 50

#### Output

[-1, -1, -1, -1, -1]

#### Explanation

All keys have the same weight, so no strictly lighter previous key exists for any chamber.

## Input Format

The first line contains a single integer n, the number of chambers.  
The second line contains n space-separated integers p_0, p_1, ..., p_[n-1], representing the weight of the obsidian key in each chamber.

## Output Format

Return array of integers. The i‑th integer should be the weight of the key in the nearest chamber j < i such that p_j < p_i. If no such chamber exists, then -1.

## Constraints

1 ≤ n ≤ 10^5  
1 ≤ p_i ≤ 10^9 for all 0 ≤ i < n.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

stack, array