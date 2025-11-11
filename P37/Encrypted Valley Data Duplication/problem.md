## Title

Encrypted Valley Data Duplication

## Slug

encrypted-valley-data-duplication

## Difficulty

Easy

## Description

In the hidden Encrypted Valley, the master cryptographer possesses a single original secret file. Before the next security audit, she must create exactly n additional copies of this file. Two high‑speed encryptors are available.
The first encryptor needs x seconds to duplicate one file (from the original or any existing copy), and the second encryptor needs y seconds. The cryptographer can operate either encryptor alone or both simultaneously.  
Determine the minimum amount of time required to produce at least n new copies of the secret file, starting with only the original.

## Examples

### 1

#### Input

5 1 2

#### Output

4

#### Explanation

We need 5 copies. Assume encryptor 1 takes 1 s, encryptor 2 takes 2 s.
    1. Use encryptor 1 on the original (1 s elapsed). Now we have 2 files. Need 4 more.
    2. Use encryptor 1 on original, encryptor 2 on a copy (2 s elapsed total, 1 s more). Encryptor 1 finishes. Now have 3 files. Need 3 more.
    3. Use encryptor 1 on original (3 s elapsed total, 1 s more). Encryptor 2 finishes its first copy. Now have 4 files. Need 2 more.
    4. Use encryptor 1 on original, encryptor 2 on a copy (4 s elapsed total, 1 s more). Encryptor 1 finishes. Now have 5 files. Need 1 more. Encryptor 2 finishes. Now have 6 files. We have enough copies.
Minimum time is 4 seconds.

### 2

#### Input

4 1 1

#### Output

3

#### Explanation

Need 4 copies. Both encryptors take 1 s.
    1. Use encryptor 1 on original (1 s). Have 2 files. Need 3 more.
    2. Use encryptor 1 and 2 on the available files (2 s). Have 4 files. Need 1 more.
    3. Use encryptor 1 and 2 again (3 s). Have 6 files. We have enough.
Minimum time is 3 seconds.
  
## Input Format  

- Three space-separated integers n, x, and y.

## Output Format  

- Return single integer representing the minimum time in seconds required.
  

## Constraints  

- 1 ≤ n ≤ 1e8
- 1 ≤ x, y ≤ 10

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

binary-search, math, number-theory