## Title

The Phantom Cipher

## Slug

the-phantom-cipher

## Difficulty

Easy

## Description

A secret society needs to generate a large number of encrypted messages using a newly discovered phantom cipher! The master cryptographer possesses the original plaintext and must produce exactly n additional encrypted copies before the deadline. There are two magical encryption machines available.
The first machine encrypts one message (from the original or any existing encrypted copy) in x seconds, and the second machine does it in y seconds. The cryptographers can operate either machine or both simultaneously.  
Help the master determine the minimum amount of time required to obtain at least n new encrypted messages, starting with just the original plaintext.

## Examples

### 1

#### Input

5 1 2

#### Output

4

#### Explanation

We need 5 encrypted copies. Assume machine 1 takes 1 s, machine 2 takes 2 s.
1. Use machine 1 on the original (1 s elapsed). Now we have 2 messages. Need 4 more.  
2. Use machine 1 on the original, machine 2 on a copy (2 s elapsed total, 1 s more). Machine 1 finishes. Now have 3 messages. Need 3 more.  
3. Use machine 1 on the original (3 s elapsed total, 1 s more). Machine 2 finishes its first copy. Now have 4 messages. Need 2 more.  
4. Use machine 1 on the original, machine 2 on a copy (4 s elapsed total, 1 s more). Machine 1 finishes. Now have 5 messages. Need 1 more. Machine 2 finishes. Now have 6 messages. We have enough copies.  
Minimum time is 4 seconds.

### 2

#### Input

4 1 1

#### Output

3

#### Explanation

Need 4 encrypted copies. Both machines take 1 s.
1. Use machine 1 on the original (1 s). Have 2 messages. Need 3 more.  
2. Use machine 1 and 2 on the available messages (2 s). Have 4 messages. Need 1 more.  
3. Use machine 1 and 2 again (3 s). Have 6 messages. We have enough.  
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