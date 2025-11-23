## Title

The Harmonious Vowel Chant

## Slug

the-harmonious-vowel-chant

## Difficulty

Easy

## Description

In the Temple of Aethelgard, novices learn to invoke magical barriers using ancient chants. These chants are sequences composed entirely of the five sacred vowels: 'a', 'e', 'i', 'o', and 'u'.

To ensure the magic remains stable, the High Priests have decreed a strict rule: the vowels in any chant must flow in **non-decreasing alphabetical order**. This means that for any character in the chant, the character immediately following it must be the same vowel or a vowel that comes later in the alphabet. For example, "aaeeu" and "aeiou" are valid harmonious chants, but "uea" causes magical dissonance and is forbidden.

Given an integer $n$, your task is to determine the total number of distinct valid chants of length $n$ that can be formed.

## Examples

### 1

#### Input

1

#### Output

5

#### Explanation

The valid chants of length 1 are: "a", "e", "i", "o", "u".
    
### 2

#### Input

2

#### Output

15

#### Explanation

The valid chants are: "aa", "ae", "ai", "ao", "au", "ee", "ei", "eo", "eu", "ii", "io", "iu", "oo", "ou", "uu".
Note that "ea" is invalid because 'e' comes after 'a'.

## Input Format  

- The input consists of a single integer $n$, representing the length of the chant.

## Output Format  

- Return a single integer representing the number of lexicographically sorted vowel strings of length $n$.  

## Constraints  

- 1 ≤ n ≤ 50

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

dynamic-programming, math