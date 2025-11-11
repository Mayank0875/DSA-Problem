## Title

The Hidden Byte

## Slug

hidden-byte

## Difficulty

Easy

## Description

A secret message is stored as a single byte in a secure system. The original byte can be duplicated, but the system needs exactly n additional copies of this byte before a data transmission begins. There are two cloning modules available.
The first module creates a copy of a byte in x seconds (it can copy the original or any existing copy), and the second module does the same in y seconds. The modules can be used independently or simultaneously.  
Determine the minimum amount of time required to produce at least n new copies of the byte, starting with only the original.

## Examples

### 1

#### Input

5 1 2

#### Output

4

#### Explanation

We need 5 copies. Assume module 1 takes 1 s, module 2 takes 2 s.
    1. Use module 1 on the original (1 s elapsed). Now we have 2 bytes. Need 4 more.
    2. Use module 1 on original, module 2 on a copy (2 s elapsed total, 1 s more). Module 1 finishes. Now have 3 bytes. Need 3 more.
    3. Use module 1 on original (3 s elapsed total, 1 s more). Module 2 finishes its first copy. Now have 4 bytes. Need 2 more.
    4. Use module 1 on original, module 2 on a copy (4 s elapsed total, 1 s more). Module 1 finishes. Now have 5 bytes. Need 1 more. Module 2 finishes. Now have 6 bytes. We have enough copies.
Minimum time is 4 seconds.

### 2

#### Input

4 1 1

#### Output

3

#### Explanation

Need 4 copies. Both modules take 1 s.
    1. Use module 1 on original (1 s). Have 2 bytes. Need 3 more.
    2. Use module 1 and 2 on the available bytes (2 s). Have 4 bytes. Need 1 more.
    3. Use module 1 and 2 again (3 s). Have 6 bytes. We have enough.
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