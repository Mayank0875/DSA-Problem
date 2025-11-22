## Title
The Galactic Treasury

## Slug
the-galactic-treasury

## Difficulty
Medium

## Description
You are the Chief Treasurer of the Galactic Empire, responsible for managing the credits stored in various treasury vaults. You are given an integer array `vaults`, where each element represents the current credit balance in a specific vault.

Throughout the day, a series of transactions occur, represented by a 2D integer array `transactions`. Each transaction is given as `[amount, vault_index]`. For every transaction, you must add the `amount` to the vault located at `vault_index`.

The Emperor has a peculiar superstition: he believes that only vaults with an even number of credits are "stable." After every single transaction, he demands a report of the total sum of credits currently held in all stable (even-valued) vaults.

Your task is to process all transactions in order and return an array containing the sum of even-valued vaults after each update.

## Examples
### 1
#### Input
[1, 2, 3, 4]
[[1, 0], [-3, 1], [-4, 0], [2, 3]]
#### Output
[8, 6, 2, 4]
#### Explanation
Initially, the array is `[1, 2, 3, 4]`.
1. Add 1 to `vaults[0]`: Array becomes `[2, 2, 3, 4]`. Sum of evens: $2 + 2 + 4 = 8$.
2. Add -3 to `vaults[1]`: Array becomes `[2, -1, 3, 4]`. Sum of evens: $2 + 4 = 6$.
3. Add -4 to `vaults[0]`: Array becomes `[-2, -1, 3, 4]`. Sum of evens: $-2 + 4 = 2$.
4. Add 2 to `vaults[3]`: Array becomes `[-2, -1, 3, 6]`. Sum of evens: $-2 + 6 = 4$.

### 2
#### Input
[1]
[[4, 0]]
#### Output
[0]
#### Explanation
Initially, the array is `[1]`.
1. Add 4 to `vaults[0]`: Array becomes `[5]`. Sum of evens: 0.

## Input Format
- The first line contains an integer $n$, the number of vaults.
- The second line contains $n$ space-separated integers representing `vaults`.
- The third line contains an integer $q$, the number of transactions.
- The next $q$ lines each contain two space-separated integers representing the `amount` and `vault_index` for a transaction.

## Output Format
Return array of size $q$ representing the sum of even values after each transaction.

## Constraints

- 1 ≤ N ≤ 10^4
- -1e4 ≤ arr[i] ≤ 1e4
- 1 ≤ q ≤ 10^4
- -1e4 ≤ val ≤ 1e4
- 0 ≤ index[i] ≤ n


## Time Limit
1 second

## Memory Limit
256 MB

## Tags
array