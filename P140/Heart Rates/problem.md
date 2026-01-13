## Title
Heart Rates

## Slug
heart-rates

## Difficulty
Easy

## Description
A fitness class monitors participants' heart rates.

The monitor records the BPM of $N$ participants in an array. To gauge intensity, the instructor needs to assign a rank to every participant based on its BPM.

The ranking rules are simple: the participant with the **smallest** BPM gets **Rank 1**. The next distinct BPM gets **Rank 2**, and so on.

If two or more participants have the exact same BPM, they must receive the **same rank**. The ranks must be integers starting from 1.

Your task is to replace each participant's BPM with its corresponding rank.

## Examples

### 1

#### Input
4
40 10 20 30

#### Output
4 1 2 3

#### Explanation
10 is the smallest (Rank 1). 20 is the second smallest (Rank 2). 30 is third (Rank 3). 40 is largest (Rank 4).

### 2

#### Input
3
2 2 2

#### Output
1 1 1

#### Explanation
All participants share the same BPM, so they share Rank 1.

## Input Format
- The first line contains an integer `n`, the number of participants.
- The second line contains `n` space-separated integers representing the BPMs.

## Output Format
- Return an array of integers where each element is the rank of the corresponding participant.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ values ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, hash-table, sorting
