## Title
Internet Speeds

## Slug
internet-speeds

## Difficulty
Easy

## Description
A user tests download speeds from different ISPs.

The speed test records the speed (Mbps) of $N$ ISPs in an array. To choose a provider, the user needs to assign a rank to every ISP based on its speed (Mbps).

The ranking rules are simple: the ISP with the **smallest** speed (Mbps) gets **Rank 1**. The next distinct speed (Mbps) gets **Rank 2**, and so on.

If two or more ISPs have the exact same speed (Mbps), they must receive the **same rank**. The ranks must be integers starting from 1.

Your task is to replace each ISP's speed (Mbps) with its corresponding rank.

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
All ISPs share the same speed (Mbps), so they share Rank 1.

## Input Format
- The first line contains an integer `n`, the number of ISPs.
- The second line contains `n` space-separated integers representing the speed (Mbps)s.

## Output Format
- Return an array of integers where each element is the rank of the corresponding ISP.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ values ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, hash-table, sorting
