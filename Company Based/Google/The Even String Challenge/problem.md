## Title

The Even String Challenge

## Slug

the-even-string-challenge

## Difficulty

Medium

## Description


A string $a$ is called **even** if it consists of a concatenation (joining) of strings of length 2 consisting of the same characters. In other words, a string $a$ is even if two conditions are satisfied at the same time:
* Its length $n$ is even.
* For all odd $i$ ($1 \le i \le n-1$), $a_i = a_{i+1}$ is satisfied.

For example, the following strings are even: "" (empty string), "tt", "aabb", "oooo", and "ttrrrroouuuuuuuukk". The following strings are not even: "aaa", "abab", and "abba".

Given a string $s$ consisting of lowercase Latin letters, find the **minimum number of characters** to remove from the string $s$ to make it even. The deleted characters do not have to be consecutive.

## Examples

### 1

#### Input

aabbdabdccc

#### Output

3

#### Explanation

You can remove the characters with indices 6, 7, and 9 (0-indexed characters 'a', 'b', 'c') to get an even string "aabbddcc".
    
### 2

#### Input

zyx

#### Output

3

#### Explanation

Each character occurs exactly once, so to get an even string, you must remove all characters (resulting in an empty string).
  

## Input Format  

- The only input line has an string s.

## Output Format  

- Return a single integer — the minimum number of characters that must be removed.
  

## Constraints  

- 1 ≤ |s| ≤ 1e5

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

string, dynamic-programming

## Company
google