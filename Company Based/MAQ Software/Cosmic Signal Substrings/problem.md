## Title

Cosmic Signal Substrings

## Slug

cosmic-signal-substrings

## Difficulty

Medium

## Description

An astronomer is analyzing signals from deep space. The base signal is an infinite, repeating pattern of the English alphabet: "...zabcdefghijklmnopqrstuvwxyzabcdefg...".

She has recorded a new signal, `s`. She needs to find out how many unique, non-empty substrings of `s` are also "contiguous" substrings of the infinite base signal.

A substring is contiguous if every character is followed by the next character in the alphabet (with 'z' wrapping around to 'a'). For example, "abc" and "za" are contiguous, but "ac" and "ca" are not.

Your task is to count these unique contiguous substrings.

## Examples

### 1

#### Input

a

#### Output

1

#### Explanation

Only the substring "a" of s is in the base signal.
    
### 2

#### Input

cac

#### Output

2

#### Explanation

There are two unique contiguous substrings ("a", "c") of s in the base signal. The substrings "ca", "ac", and "cac" are not contiguous.
  

## Input Format  

- The input consists of a single line containing the string `s`.

## Output Format  

- Return single integer representing the count of unique contiguous substrings.
  

## Constraints  

- 1 ≤ s.length ≤ 1e5
- `s` consists of lowercase English letters.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

dynamic-programming, string