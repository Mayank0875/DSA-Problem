## Title

Previous Higher Encryption Level

## Slug

previous-higher-encryption-level

## Difficulty

Easy

## Description

Imagine traversing the Encrypted Valley, a line of data vaults each protected by an encryption strength. As you stand before each vault, you look back (to your left) and want to know the strength of the nearest vault that has a strictly higher encryption level than the one you are currently facing. If all previous vaults are weaker or have equal strength, or if it's the first vault, there is no such stronger vault to the left. Your goal is to determine this stronger vault's encryption strength for each position along the valley.

## Examples

### 1

#### Input

8
[30, 60, 90, 50, 80, 40, 70, 50]

#### Output

[-1, -1, -1, 90, 90, 80, 80, 70]

#### Explanation

Vault 0 (30): No previous vault. Output -1.  
Vault 1 (60): Vault 0 (30) is weaker. Output -1.  
Vault 2 (90): Vaults 0 (30), 1 (60) are weaker. Output -1.  
Vault 3 (50): Vault 2 (90) is the nearest stronger. Output 90.  
Vault 4 (80): Vault 2 (90) is the nearest stronger. Output 90.  
Vault 5 (40): Vault 4 (80) is the nearest stronger. Output 80.  
Vault 6 (70): Vault 4 (80) is the nearest stronger. Output 80.  
Vault 7 (50): Vault 6 (70) is the nearest stronger. Output 70.

### 2

#### Input

5
50 50 50 50 50

#### Output

[-1, -1, -1, -1, -1]

#### Explanation

All vaults have equal encryption strength, so no strictly stronger previous vault exists.

## Input Format

The first line contains a single integer n, the number of vaults.  
The second line contains n space-separated integers h_0, h_1, ..., h_[n-1], representing the encryption strength of each vault.

## Output Format

Return array of integers. The i-th integer should be the strength of the nearest vault j < i such that h_j > h_i. If no such day exists, then -1.

## Constraints

1 ≤ n ≤ 10^5  
1 ≤ h_i ≤ 10^9 for all 0 ≤ i < n.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

stack, array