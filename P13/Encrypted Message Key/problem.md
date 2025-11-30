## Title

Encrypted Message Key

## Slug

encrypted-message-key

## Difficulty

Easy

## Description

You are a cryptographer trying to break a code. You have a sorted list
of possible decryption keys. You need to check if your `target` key is
in this list. Return 1 if the key is present otherwise 0. You must write
an algorithm with O(log n) runtime complexity.


## Examples

### 1

#### Input

6 8
[2, 5, 7, 8, 11, 12]


#### Output

1

#### Explanation

The target ID 8 is found in the lists.

### 2

#### Input

6 6
[2, 5, 7, 8, 11, 12]

#### Output

0

#### Explanation

The target ID 6 is not found in the list.

## Input Format

- The first line contains an integers n and target , the number of keys and the key to find. 
- The second line contains n space-separated integers representing the sorted description keys.

## Output Format

- Return 1 if the target is found, and 0 otherwise.

## Constraints

- 1 ≤ n ≤ 10^5
- 1 ≤ keys, target ≤ 10^9
- The description keys are sorted in non-decreasing order.

## Time Limit

1 second

## Memory Limit

256 MB

## Tags

binary-search, array
