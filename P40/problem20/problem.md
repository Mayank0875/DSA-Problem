## Title

Next Higher Encryption Level in Encrypted Valley

## Slug

next-higher-encryption-level

## Difficulty

Easy

## Description

The inhabitants of Encrypted Valley are analyzing the security levels of a sequence of vaults to plan future upgrades. For each vault, they want to identify the security level of the nearest future vault that has a strictly higher encryption level. This helps them understand security progression trends or pinpoint critical upgrade points. If no future vault has a higher encryption level (either because it is the last vault or all subsequent vaults have lower or equal levels), this should be noted. Can you calculate this for each vault?

## Examples

### 1

#### Input

8
[500, 400, 600, 300, 700, 450, 800, 500]

#### Output

[600, 600, 700, 700, 800, 800, -1, -1]

#### Explanation

Vault 0 (500): Next higher is 600 (Vault 2). Output 600.
Vault 1 (400): Next higher is 600 (Vault 2). Output 600.
Vault 2 (600): Next higher is 700 (Vault 4). Output 700.
Vault 3 (300): Next higher is 700 (Vault 4). Output 700.
Vault 4 (700): Next higher is 800 (Vault 6). Output 800.
Vault 5 (450): Next higher is 800 (Vault 6). Output 800.
Vault 6 (800): No future vault is higher. Output -1.
Vault 7 (500): No future vault exists. Output -1.

### 2

#### Input

5
50 50 50 50 50

#### Output

[-1, -1, -1, -1, -1]

#### Explanation

All encryption levels are equal, so no future vault has a higher level.

## Input Format

The first line contains a single integer n, the number of vaults.
The second line contains n space-separated integers a_0, a_1, ..., a_[n-1], representing the encryption level for each vault.

## Output Format

Return array of integers. The i-th integer should be the encryption level of the nearest vault j > i such that a_j > a_i. If no such day exists, then -1.

## Constraints

1 ≤ n ≤ 10^5
1 ≤ a_i ≤ 10^9 for all 0 ≤ i < n.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

stack, array